# Release Checklist

Follow these step-by-step tasks to release and maintain your open source project using the MIT license. Ensure you complete each item before moving on to the next:

1.  [ ] Register your release:
   - Use the [Open Source Portal](https://repos.opensource.microsoft.com/release) to register your intended release.
   - This will trigger a review by CELA and management.

2. [ ] Create and initialize a GitHub repository:
   - [Create your GitHub repository](https://docs.opensource.microsoft.com/releasing/release-on-github/repo-creation) using the [repository wizard](https://repos.opensource.microsoft.com/microsoft/new).
   - Repositories must be hosted within a 1ES-managed GitHub organization and may not be made public until the release registration is approved by CELA and management.
   - Include the following in the root directory:
      - A README.md file describing the purpose and state of the repository, including third-party code information.
      - A LICENSE.txt file with the [MIT license text](https://docs.opensource.microsoft.com/releasing/general-guidance/boilerplate-license-files). (Other licenses must be cleared with CELA.)
      - A CONTRIBUTING.md file with instructions for contributing to the project, including Microsoft's Contributor License Agreement and technical guidance.
      - A SECURITY.md file using the [repo-templates/SECURITY.md template](https://github.com/microsoft/repo-templates/blob/main/shared/SECURITY.md).
      - A CODE_OF_CONDUCT.md file using the [repo-templates/CODE_OF_CONDUCT.md template](https://github.com/microsoft/repo-templates/blob/main/shared/CODE_OF_CONDUCT.md).
      - Consider adding a SUPPORT.md file using the [repo-templates/SUPPORT.md template](https://github.com/microsoft/repo-templates/blob/main/projections/mit/SUPPORT.md).
      - Telemetry Notice: If the release has code that enables Microsoft to collect telemetry, provide instructions to turn off the telemetry and include the [telemetry/data collection notice](https://docs.opensource.microsoft.com/releasing/general-guidance/telemetry) in the README.md file.
      - Trademark Notice: Include the provided Trademark notice in your README.md, ensuring proper use of Microsoft trademarks and logos.
      - Security Reporting Instructions: Include instructions for privately reporting security vulnerabilities found in your project.
      - Consider registering a domain name for your project following the [open source project domain name guidance](https://docs.opensource.microsoft.com/releasing/prepare-for-release/project-naming-and-domain-names#open-source-project-domain-name-guidance).

3. [ ] Prepare the code for release:
   - Ensure the code is licensed under the MIT license by including the [language-appropriate comment](https://docs.opensource.microsoft.com/releasing/general-guidance/copyright-headers) at the head of each source file.
   - Remove sensitive assets, such as internal or confidential information, internal paths, tools, codenames, proprietary fonts, internal telemetry, and email aliases.
   - Remove any trademarks or product icons.
   - Follow the [going public guidance](https://docs.opensource.microsoft.com/releasing/general-guidance/going-public) to prepare the code and commit history for publication, including running PoliCheck.
   - Follow your organization's Secure Development Lifecycle (SDL) process or use 1CS for any required security and threat model reviews.
   - If your repository includes third-party OSS, describe its use and its license in a NOTICE file. Consult with OSS CELA when in doubt.

4. [ ] Publish the code:
   - Once your registration and review process is complete, make your GitHub repository public.

5. [ ] Going forward, ensure:
   - [ ] Further Microsoft Contributions:
     - File a [contribution request](https://docs.opensource.microsoft.com/contributing/third-party) if the feature you are adding is outside the scope of your original release request or if you are adding non-open source Microsoft code that your team did not author.
   - [ ] Staffing:
     - Ensure at least one team member is committed to managing community interactions, merging pull requests, giving feedback, and releasing new versions.
   - [ ] Buildable & Runnable:
     - Make sure your project is easy to build and has binaries available, as this is essential for attracting contributors.
   - [ ] Security:
     - Ensure your project follows your organization's SDL requirements and expectations for security reviews, responding to security alerts, and other best practices for product/service development.
   - [ ] Foster your community:
     - Look for ways to continue engagement with potential contributors and foster a thriving community.

By following these guidelines, you can release your open source project using the MIT license and maintain it successfully while complying with Microsoft's policies and standards.