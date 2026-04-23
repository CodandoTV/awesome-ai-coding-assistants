# OWASP Mobile Security Skill

## Skill Description

This skill provides essential resources and guidance derived from the OWASP Mobile Security Project. It encompasses best practices, testing methodologies, and security verification standards crucial for developing and securing mobile applications. Utilize this skill to identify, understand, and mitigate common mobile security vulnerabilities.

## Installation

This skill can be installed using various AI CLI tools. The specific commands may vary slightly depending on the CLI and its version.

### Gemini CLI

The Gemini CLI supports installing skills in several ways.

**1. Direct Installation from a Skill File URL:**
You can install the skill directly from its `.skill` file URL if it's hosted online.
```bash
gemini skills install https://github.com/CodandoTV/awesome-ai-coding-assistants/skills/owasp-mobile-security/owasp-mobile-security.skill
```

**2. Installation from a Git Repository:**
If the skill is part of a larger Git repository, you can install it by providing the repository URL and the path to the skill file within the repository.
```bash
# Replace <repository_url> with the actual repository URL (e.g., https://github.com/CodandoTV/awesome-ai-coding-assistants.git)
# The --path argument specifies the directory containing the .skill file relative to the repository root.
gemini skills install https://github.com/CodandoTV/awesome-ai-coding-assistants.git --path skills/owasp-mobile-security
```
After installation, you may need to reload skills:
```bash
/skills reload
```
Then, activate the skill:
```bash
gemini activate owasp-mobile-security
```

### Other Major CLIs (Examples)

These are example commands and may differ based on the specific CLI's implementation. Refer to the official documentation for precise instructions. To install this specific skill directly, it's recommended to clone the repository and then install from its local path.

*   **Claude Code:**
    To install this skill directly, clone the repository and use the local path:
    1. Clone the repository:
       ```bash
       git clone https://github.com/CodandoTV/awesome-ai-coding-assistants.git
       ```
    2. Navigate to the cloned repository directory.
    3. Install the skill using its local path:
       ```bash
       claude skills install ./skills/owasp-mobile-security/
       ```
    (Consult Claude Code documentation for exact commands and paths.)

*   **GitHub Copilot CLI:**
    To install this skill directly, clone the repository and use the local path:
    1. Clone the repository:
       ```bash
       git clone https://github.com/CodandoTV/awesome-ai-coding-assistants.git
       ```
    2. Navigate to the cloned repository directory.
    3. Install the skill using its local path:
       ```bash
       copilot skills install ./skills/owasp-mobile-security/
       ```
    (Consult GitHub Copilot CLI documentation for exact commands and paths.)

*   **Cursor:**
    Cursor may have specific commands for adding skills. A common pattern to target this skill directly is to clone the repository and add it as a local skill:
    1. Clone the repository:
       ```bash
       git clone https://github.com/CodandoTV/awesome-ai-coding-assistants.git
       ```
    2. Navigate to the cloned repository directory.
    3. Add the skill using its local path:
       ```bash
       cursor skills add ./skills/owasp-mobile-security/
       ```
    (Consult Cursor's documentation for adding custom skills or plugins.)

*   **Windsurf:**
    To install this skill directly, clone the repository and use the local path:
    1. Clone the repository:
       ```bash
       git clone https://github.com/CodandoTV/awesome-ai-coding-assistants.git
       ```
    2. Navigate to the cloned repository directory.
    3. Install the skill using its local path:
       ```bash
       windsurf skills install ./skills/owasp-mobile-security/
       ```
    (Consult Windsurf documentation for exact commands and paths.)

*   **OpenCode:**
    To install this skill directly, clone the repository and use the local path:
    1. Clone the repository:
       ```bash
       git clone https://github.com/CodandoTV/awesome-ai-coding-assistants.git
       ```
    2. Navigate to the cloned repository directory.
    3. Install the skill using its local path:
       ```bash
       opencode skills install ./skills/owasp-mobile-security/
       ```
    (Consult OpenCode documentation for exact commands and paths.)

---

# Skill de Segurança Mobile OWASP

## Descrição da Skill

Esta skill oferece recursos e orientações essenciais derivadas do OWASP Mobile Security Project. Ela abrange melhores práticas, metodologias de teste e padrões de verificação de segurança cruciais para o desenvolvimento e a segurança de aplicações mobile. Utilize esta skill para identificar, entender e mitigar vulnerabilidades comuns de segurança mobile.

## Instalação

Esta skill pode ser instalada usando várias ferramentas de CLI de IA. Os comandos específicos podem variar ligeiramente dependendo da CLI e de sua versão.

### Gemini CLI

A Gemini CLI suporta várias formas de instalar skills.

**1. Instalação Direta de uma URL de Arquivo de Skill:**
Você pode instalar a skill diretamente de sua URL de arquivo `.skill` se ela estiver hospedada online.
```bash
gemini skills install https://github.com/CodandoTV/awesome-ai-coding-assistants/skills/owasp-mobile-security/owasp-mobile-security.skill
```

**2. Instalação de um Repositório Git:**
Se a skill faz parte de um repositório Git maior, você pode instalá-la fornecendo a URL do repositório e o caminho para o arquivo de skill dentro do repositório.
```bash
# Substitua <repository_url> pela URL real do repositório (ex: https://github.com/CodandoTV/awesome-ai-coding-assistants.git)
# O argumento --path especifica o diretório que contém o arquivo .skill em relação à raiz do repositório.
gemini skills install https://github.com/CodandoTV/awesome-ai-coding-assistants.git --path skills/owasp-mobile-security
```
Após a instalação, você pode precisar recarregar as skills:
```bash
/skills reload
```
Em seguida, ative a skill:
```bash
gemini activate owasp-mobile-security
```