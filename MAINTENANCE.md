# Maintenance

## Update the GitHub actions
It's a good idea to regularly check the action versions in your repositories for updates:
1. Pick one:
   * Open the [ci.yml file](https://github.com/sphinx-playground/sphinx-single/blob/master/.github/workflows/ci.yml) in the **sphinx-single** repository.
   * Open the [ci.yml file](https://github.com/sphinx-playground/sphinx-split-host/blob/master/.github/workflows/ci.yml) in the **sphinx-split-host** repository.
2. Do a search for each of these actions in the file and compare their versions against the versions listed in their action repositories:
   * **actions/checkout:**
     * GitHub Marketplace: [https://github.com/marketplace/actions/checkout](https://github.com/marketplace/actions/checkout)
     * Repository: [https://github.com/actions/checkout](https://github.com/actions/checkout)
     * Releases: [https://github.com/actions/checkout/releases](https://github.com/actions/checkout/releases)
   * **actions/deploy-pages:**
     * GitHub Marketplace: [https://github.com/marketplace/actions/deploy-github-pages-site](https://github.com/marketplace/actions/deploy-github-pages-site)
     * Repository: [https://github.com/actions/deploy-pages](https://github.com/actions/deploy-pages)
     * Releases: [https://github.com/actions/deploy-pages/releases](https://github.com/actions/deploy-pages/releases)
   * **actions/setup-python:**
     * GitHub Marketplace: [https://github.com/marketplace/actions/setup-python](https://github.com/marketplace/actions/setup-python)
     * Repository: [https://github.com/actions/setup-python](https://github.com/actions/setup-python)
     * Releases: [https://github.com/actions/setup-python/releases](https://github.com/actions/setup-python/releases)
   * **actions/upload-pages-artifact:**
     * GitHub Marketplace: [https://github.com/marketplace/actions/upload-github-pages-artifact](https://github.com/marketplace/actions/upload-github-pages-artifact)
     * Repository: [https://github.com/actions/upload-pages-artifact](https://github.com/actions/upload-pages-artifact)
     * Releases: [https://github.com/actions/upload-pages-artifact/releases](https://github.com/actions/upload-pages-artifact/releases)
3. Check the **GitHub Marketplace** or **Repository** pages for each action for its latest version and for possible information on deprecated or updated configurations that may need to be added, adjusted, or removed to accommodate the new versions.
4. Verify the accuracy of the latest version by comparing the versions in each **Description** page with the version at the top of its **Releases** pages since the examples in the **Description** pages aren't always kept up-to-date.
5. Once you've chosen a new version, update the version number in the **ci.yml** file and, if necessary, make the additions, adjustments, or removals to accommodate the new version.

## Update the Python version
It's a good idea to regularly check the Python version in your repositories for updates:
1. Pick one:
   * Open the [ci.yml file](https://github.com/sphinx-playground/sphinx-single/blob/master/.github/workflows/ci.yml) in the **sphinx-single** repository.
   * Open the [ci.yml file](https://github.com/sphinx-playground/sphinx-split-host/blob/master/.github/workflows/ci.yml) in the **sphinx-split-host** repository.
2. Do a search for **python-version** in the file and compare its version against the Python versions listed in the [Python downloads](https://www.python.org/downloads) or [Status of Python Versions](https://devguide.python.org/versions) page to see if it's still supported by Python.
3. If it's not, check the latest version against the **GitHub Actions Runner Images** to ensure that it's supported by GitHub for your image:
   1. Go to the [GitHub Actions Runner Images](https://github.com/actions/runner-images#available-images) page.
   2. Scroll down to the **Available Images** section of the page.
   3. Open the **Included Software** link for your image (for example, the latest **Ubuntu** release).
   4. Scroll down to the **Cached Tools** section.
   5. Scroll down to the **Python** section inside of that section.
   6. Jot down all of the **Python** versions.
4. Once you've chosen a new version, check the [https://www.python.org/doc/versions](https://www.python.org/doc/versions) page for possible information about deprecated or updated configurations that may need to be added, adjusted, or removed to accommodate that new version.
5. Update the version number in the **ci.yml** file and make the accommodations, if necessary.
