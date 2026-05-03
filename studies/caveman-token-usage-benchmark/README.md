# Caveman Token Usage Benchmark

This study was created while preparing a video for [CodandoTV](https://www.youtube.com/@CodandoTV) about [Caveman](https://github.com/JuliusBrussee/caveman) and its real impact on token usage inside Claude Code.

The main question was simple:

> Does Caveman really reduce token usage, or does it mostly reduce response verbosity?

This folder contains the raw Claude Code logs and visual summaries used in the study.

## Structure

```text
data/
  Raw Claude Code terminal logs.

image/
  Visual summaries with charts, tables, and final context screenshots.
```

## Test Groups

The study compares:

- Random questions vs code questions
- Portuguese vs English prompts
- Caveman disabled vs Caveman full mode
- Caveman full vs ultra mode

---

## 1. Code Questions: No Caveman vs Caveman Full

![Code questions PT: Caveman off vs full](image/code-questions-pt-compare-cave-off-full.png)

Logs:

- [`code-questions-pt-cave-off.txt`](data/code-questions-pt-cave-off.txt)
- [`code-questions-pt-cave-full.txt`](data/code-questions-pt-cave-full.txt)

Summary:

Caveman full increased token usage in code tasks. The final context went from **33.7k** to **40.2k**.

---

## 2. Random Questions: No Caveman vs Caveman Full

![Random questions PT: Caveman off vs full](image/random-questions-pt-compare-cave-off-full.png)

Logs:

- [`random-questions-pt-cave-off.txt`](data/random-questions-pt-cave-off.txt)
- [`random-questions-pt-cave-full.txt`](data/random-questions-pt-cave-full.txt)

Summary:

Caveman full slightly reduced usage in random questions. The final context went from **27.7k** to **27.4k**.

---

## 3. Code Questions: Portuguese vs English with Caveman

![Code questions EN vs PT with Caveman](image/code-questions-en-cave-full.png)

Logs:

- [`code-questions-pt-cave-full.txt`](data/code-questions-pt-cave-full.txt)
- [`code-questions-en-cave-full.txt`](data/code-questions-en-cave-full.txt)

Summary:

English performed better in code tasks with Caveman. The final context dropped from **40.2k** to **35.2k**.

---

## 4. Random Questions: Portuguese vs English with Caveman

![Random questions EN vs PT with Caveman](image/random-questions-en-cave-full.png)

Logs:

- [`random-questions-pt-cave-full.txt`](data/random-questions-pt-cave-full.txt)
- [`random-questions-en-cave-full.txt`](data/random-questions-en-cave-full.txt)

Summary:

English did not help for random questions. The final context increased from **27.4k** to **29.0k**.

---

## 5. Code Questions: Caveman Full vs Ultra

![Code questions EN: Caveman full vs ultra](image/code-questions-en-cave-ultra.png)

Logs:

- [`code-questions-en-cave-full.txt`](data/code-questions-en-cave-full.txt)
- [`code-questions-en-cave-ultra.txt`](data/code-questions-en-cave-ultra.txt)

Summary:

Ultra mode did not reduce token usage in code tasks. The final context increased from **35.2k** to **38.8k**.

---

## 6. Random Questions: Caveman Full vs Ultra

![Random questions EN: Caveman full vs ultra](image/random-questions-en-cave-ultra.png)

Logs:

- [`random-questions-en-cave-full.txt`](data/random-questions-en-cave-full.txt)
- [`random-questions-en-cave-ultra.txt`](data/random-questions-en-cave-ultra.txt)

Summary:

Ultra mode also did not reduce token usage in random questions. The final context increased from **29.0k** to **29.8k**.

---

## Main Findings

- Caveman can reduce verbosity, but not always total context usage.
- For random questions in Portuguese, the reduction was small.
- For code questions in Portuguese, Caveman used more context.
- English helped in code tasks, but not in random questions.
- Ultra mode was not cheaper in these tests.
- In Claude Code, most cost seems to come from context, tool usage, file reads, and repository analysis, not only from response length.

## Final Takeaway

Caveman is useful to change the response style, but it is not a guaranteed token saver.

For code tasks, especially inside Claude Code, reducing verbosity is not the same as reducing the real cost of the session.

## Video

This study was also used as supporting material for a video on the CodandoTV channel:

[CodandoTV on YouTube](https://www.youtube.com/@CodandoTV)
