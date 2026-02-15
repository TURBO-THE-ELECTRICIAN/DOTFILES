## gemini suggestions 
To build a truly **Sovereign Developer Environment** for an electrician/coder, your dotfiles shouldn't just be about aesthetics—they should be about **Utility, Reference, and Compliance**.

Here is a list of specialized dotfiles (and configurations) designed for the **SparkAI** ecosystem.

-----

### 1\. `.bash_aliases` (The "Shortcut" File)

The core of your efficiency. This turns 50-character commands into 3-character "rizz."

```bash
# NEC Article Lookups
alias nec="python3 ~/ELECTRICIAN/spark_lookup.py"
alias loadcalc="python3 ~/ELECTRICIAN/LOAD-CALCS/main.py"

# Quick Persona Audits
alias audit="bash ~/Script-tools/audit_files.sh"

# Compliance Check (The "Vader" Move)
alias check-ground="nec --query '250.66'"
alias check-fill="nec --query 'Table 1'"

# Navigation
alias lab="cd ~/AiLab"
alias boss="cd ~/ELECTRICIAN-INDEX"
```

-----

### 2\. `.vimrc` / `init.lua` (The "Blueprint" Editor)

Configure your editor to treat `.py` and `.json` files like high-stakes electrical diagrams.

  * **Highlighting:** Set custom colors for NEC keywords (e.g., `BONDING`, `GROUNDING`, `AMPERAGE`).
  * **Linters:** Integrate `flake8` or `pylint` to catch "beta" math errors before you save.
  * **Abbreviations:**
      * `iab nec23 # NEC 2023 Compliance Verified`
      * `iab gfcireq Ground-Fault Circuit-Interrupter protection required per 210.8`

-----

### 3\. `.gitconfig` (The "Chain of Custody")

Essential for the "White Hat" audit trail. This proves who made the calculation and when.

  * **Global User:** Your "Main Character" name and professional email.
  * **Aliases:**
      * `git sigma = commit -m "Peak compliance achieved. No hallucinations."`
      * `git oops = reset --hard HEAD~1` (The "Undo the fire" command).

-----

### 4\. `.gemini_rc` or `.qwen_env` (The "AI Brain" Config)

Define how your local LLMs behave without having to prompt them every time.

```bash
# System Prompts for local inference
export SPARK_PERSONA="Act as a Master Electrician with 30 years experience. Prioritize NFPA 70 2026 standards. Keep responses concise and use trade terminology."
export AI_TEMP=0.2 # Lower temperature = less "yapping," more factual accuracy.
```

-----

### 5\. `.tmux.conf` (The "Command Center" Layout)

Divide your terminal screen into a functional electrical workstation.

  * **Pane 1:** Your Python code editor.
  * **Pane 2:** The `progress_server` running live.
  * **Pane 3:** A constant feed of the `nec_data.py` for quick reference.

-----

### 6\. `.tool-versions` (The "Compliance Version" File)

If you use `asdf` or `mise`, this ensures you are using the exact versions of Python and Node that the "Boss" approved.

  * `python 3.12.1`
  * `nodejs 20.10.0`

-----

### 7\. `.npmrc` / `.python-version`

Standardize the environment.

  * **Senior Move:** Disable telemetry in these files to keep your "Sovereign Lab" private.

-----

### 8\. `.imperial_guard` (The "Custom Linter")

A hidden dotfile in your `Script-tools` that contains a list of "Forbidden Phrases" (like the "ELECTRIAN" typo) that your scripts scan for during a push.

-----

### 🛠️ The "Grand Master" Setup

To deploy these immediately, you should create a **`dotfiles` repository** and use a tool like **`stow`** to manage them.

```bash
# Assert dominance over your home directory
cd ~/dotfiles
stow .
```

**Next Step:** Would you like me to generate a complete, copy-pasteable `.bash_aliases` file that includes the **2026 NEC $2 \text{ VA/ft}^2$** calculation logic as a one-liner command?
