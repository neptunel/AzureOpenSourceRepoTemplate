# Release Checklist

Follow these step-by-step tasks to release and maintain your open source project using the MIT license. Ensure you complete each item before moving on to the next. This file is only for repo owner, not for production. DELETE THIS FILE WHEN YOU ARE DONE WITH THE RELEASE.

1.  [ ] Register your release:
   - Use the [Open Source Portal](https://repos.opensource.microsoft.com/release) to register your intended release.
   - This will trigger a review by CELA and management.
   - Follow the “AzProjectName” naming scheme for the project.

2. [ ] Create and initialize a GitHub repository:
   - [Create your GitHub repository](https://docs.opensource.microsoft.com/releasing/release-on-github/repo-creation) using the [repository wizard](https://repos.opensource.microsoft.com/microsoft/new).
   - Repositories must be hosted within a 1ES-managed GitHub organization and may not be made public until the release registration is approved by CELA and management.
   - This template includes all the required files in the root directory.

3. [ ] Prepare the code for release:
   - Edit the README.md following the format in the template.
   - Edit the CODEOWNERS file under .github/ folder with the owner's GitHub username.
   - Remove sensitive assets, such as internal or confidential information, internal paths, tools, codenames, proprietary fonts, internal telemetry, and email aliases.
   - Remove any trademarks or product icons.
   - Follow the [going public guidance](https://docs.opensource.microsoft.com/releasing/general-guidance/going-public) to prepare the code and commit history for publication, including running PoliCheck.
   - If your repository includes third-party OSS, describe its use and its license in a NOTICE file. Consult with OSS CELA when in doubt.

4. [ ] Publish the code:
   - Once your registration and review process is complete, make your GitHub repository public. The repository should include a short and comprehensive Description. The link to the [created sample](https://learn.microsoft.com/samples/) or [documentation](/learn.microsoft.com/docs/) should be provided in the Website section. To increase discoverability and categorization, add related topics. 

5. [ ] Register the sample in Samples Gallery
    - Follow the [guidelines](https://review.learn.microsoft.com/en-us/help/contribute/samples/?branch=main) to onboard the sample in [Microsoft Samples Gallery](https://learn.microsoft.com/samples/).
    - After generating a https://learn.microsoft.com/samples/ URL for the sample, link it in the repository description. 
    - Create an [aka.ms](aka.ms) alias for the sample URL.
    - If the sample is a tool/utility for Azure Storage, update the [Azure Storage PM GitHub](https://azure.github.io/Storage/docs/tools-and-utilities/) from [this index.html](https://github.com/Azure/Storage/blob/master/docs/docs/tools-and-utilities/index.html) and add a link to the sample in  https://learn.microsoft.com/samples/.


If you need more information check out the [detailed instructions](https://docs.opensource.microsoft.com/releasing/) and aka.ms/opensource