# NorseBlue Contribution Guide

- [Bug Reports](#bug-reports)
- [Development Discussion](#development-discussion)
- [Which Branch?](#which-branch)
- [Security Vulnerabilities](#security-vulnerabilities)
- [Coding Style](#coding-style)
    - [PHPDoc](#phpdoc)
    - [StyleCI](#styleci)
- [Code of Conduct](#code-of-conduct)

<a name="bug-reports"></a>
## Bug Reports

To encourage active collaboration, we strongly encourage pull requests, not just bug reports.
Pull requests will only be reviewed when marked as "ready for review" (not in the "draft" state) and all tests for new features are passing.
Lingering, non-active pull requests left in the "draft" state will be closed after a few days.

However, if you file a bug report, your issue should contain a title and a clear description of the issue.
You should also include as much relevant information as possible and a code sample that demonstrates the issue.
The goal of a bug report is to make it easy for yourself - and others - to replicate the bug and develop a fix.

Remember, bug reports are created in the hope that others with the same problem will be able to collaborate with you on solving it.
Do not expect that the bug report will automatically see any activity or that others will jump to fix it.
Creating a bug report serves to help yourself and others start on the path of fixing the problem.
If you want to chip in, you can help out by fixing [any bugs listed in our issue trackers][issue_tracker]. You must be authenticated with GitHub to view all of Laravel's issues.

NorseBlue's source code is managed on GitHub, and there are repositories for each of project which you can find [here][github_profile].

<a name="development-discussion"></a>
## Development Discussion

You may propose new features or improvements of existing NorseBlue projects in the proper repository's GitHub discussion board.
If you suggest a new feature, please be willing to implement at least some code that would be needed to complete the feature.

<a name="which-branch"></a>
## Which Branch?

**All** bug fixes should be sent to the latest version that supports bug fixes.
Bug fixes should **never** be sent to the `main` branch unless they fix features that exist only in the upcoming release.

**Minor** features that are **fully backward compatible** with the current release may be sent to the latest stable branch.

**Major** new features or features with breaking changes should always be sent to the `main` branch, which contains the upcoming release.

<a name="security-vulnerabilities"></a>
## Security Vulnerabilities

Please review our [Security/Vulnerability Policy][security_policy].

<a name="coding-style"></a>
## Coding Style

NorseBlue follows the [PSR-12][psr_12] coding standard and the [PSR-4][psr_4] autoloading standard.

<a name="phpdoc"></a>
### PHPDoc

Below is an example of a valid documentation block.
Note that the `@param` attribute is followed by two spaces, the argument type, two more spaces, and finally the variable name:

    /**
     * Register a binding with the container.
     *
     * @param  string|array  $abstract
     * @param  \Closure|string|null  $concrete
     * @param  bool  $shared
     * @return void
     *
     * @throws \Exception
     */
    public function bind($abstract, $concrete = null, $shared = false)
    {
        //
    }

<a name="styleci"></a>
### StyleCI

Don't worry if your code styling isn't perfect!
[StyleCI][styleci_link] will automatically merge any style fixes into our repositories after pull requests are merged.
This allows us to focus on the content of the contribution and not the code style.

<a name="code-of-conduct"></a>
## Code of Conduct

Please have a read at our [Code of Conduct][code_of_conduct].


[code_of_conduct]: CODE_OF_CONDUCT.md
[github_profile]: https://github.com/orgs/norse-blue/repositories
[issue_tracker]: https://github.com/issues?q=is%3Aopen+is%3Aissue+label%3Abug+user%3Anorse-blue
[psr_4]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md
[psr_12]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-12-extended-coding-style-guide.md
[security_contact]: mailto:security@norse.blue
[security_policy]: SECURITY.md
[styleci_link]: https://styleci.io
