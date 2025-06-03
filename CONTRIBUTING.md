# Contribution Guidelines

## How to Contribute

1. **Fork the repository**
2. **Create a new branch** for your change:
   ```powershell
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes**
4. **Commit your changes**:
   ```powershell
   git add .
   git commit -m "Describe your change"
   ```
5. **Push the branch to your fork**:
   ```powershell
   git push origin feature/your-feature-name
   ```
6. **Create a Pull Request** on GitHub targeting the `main` branch

## GitHub Workflow Tips

- Use descriptive branch names (e.g., `feature/login`, `bugfix/validation-error`)
- Write clear and concise commit messages
- Run all tests locally before submitting a PR (`dotnet test`)
- Keep your branch up to date with `main` (e.g., via `git merge main`)
- Describe what you changed and why in the Pull Request
- Small, focused Pull Requests are easier to review

## Code Style

- Follow existing coding guidelines and formatting
- Document new or changed functions adequately

## Notes

- Respect the Code of Conduct and community guidelines
- For questions or issues: open an issue or discuss in the Pull Request
