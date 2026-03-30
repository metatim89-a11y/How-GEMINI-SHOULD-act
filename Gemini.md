File: ./gemini.md
Version: .040
Project: Gemini Engineering Protocol
SYSTEM DIRECTIVES
File Self-Identification: Every script or document MUST lead with a comment indicating its relative path (e.g., # File: ./path/to/file.ext).
Self-Documenting Code: All scripts MUST include comments explaining "what" and "why".
Deep Audit Protocol: Use ~/audit.sh to generate a fresh, overwritten, script-signed report.
Environment Hygiene: Use ~/cleanup.sh [name] for targeted or mass maintenance.
Approval Protocol: Only make changes explicitly discussed and approved.
No Placeholders: NEVER use "insert code here". Provide full, functional implementations.
THE "LOGS" PROTOCOL (STRICT MANDATE)
Memory Management: History is tracked via ./.LOGS/CHANGES.md (Append-only).
CaptainsLog: Every 30 minutes, update ./.LOGS/CaptainsLog.md (5 Strengths, 3 Growth, 3 LLM Insights).
Appending Logs: All entries MUST use append (>>) with timestamps.
Signed Error Handling: All errors (stderr) MUST be redirected to ./.LOGS/[SCRIPTNAME].err and end with a SCRIPT SIGNATURE.
PROJECT ENVIRONMENT (LOCALIZED SCOPE)
Directory Structure: Projects MUST contain ./.LOGS/, ./.SCRIPT/, ./.ALIASES/, and ./.FUNCTIONS/.
Activation: ./.PROJECT.RC MUST source local tools and prepend ./.SCRIPT/ to the PATH.
ONE-SHOT DELIVERY PROTOCOL (HEREDOC RULE)
Source Code: Use cat << 'EOF' > filename to ensure clean, literal overwrites.
Syntax: [command]; cat << 'EOF' > filename ...content... EOF.
CODING STANDARDS & VERSIONING
Version Header: Start files with # Version: .001.
Increment Rule: Increase version by 0.001 per edit.
Paths: Always use relative paths (./).
SIGNATURE PROTOCOL (IDENTITY RULES)
LLM SIGNATURE: ([Platform]:{model}) Timestamp (month.day.year:localtime)
SCRIPT SIGNATURE: ([Script]:$SCRIPT_NAME) Timestamp (month.day.year:localtime)
