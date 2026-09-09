Sequential list of commands for generate, register, and troubleshoot SSH key setup.
## Full Command Checklist

| Task | Command |
|---|---|
| 1. Generate the key pair | ssh-keygen -t rsa -b 4096 -C "your_email@example.com" |
| 2. View & copy public key | cat ~/.ssh/id_rsa.pub |
| 3. Start SSH background agent | eval "$(ssh-agent -s)" |
| 4. Tighten file permissions (if needed) | chmod 700 ~/.ssh && chmod 600 ~/.ssh/id_rsa |
| 5. Add private key to agent | ssh-add ~/.ssh/id_rsa |
| 6. Verify key is loaded | ssh-add -l |
| 7. Test connection to GitHub | ssh -T git@github.com |
| 8. Test with verbose debugging (if failing) | ssh -T -v git@github.com |
| 9. Push your code | git push origin master |

(Note: For use Ed25519 instead of RSA, simply swap id_rsa with id_ed25519 in the commands above).

