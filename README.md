This repository contains a set of linters for your Symfony projects:
* PHP Mess Detector
* PHP Code Sniffer

## Installation

Install dependencies:

`composer install`

PHPMD:

Configure it in your phpstorm:

1. Settings -> search for `phpmd` in the search bar
2. Go to the editor -> inspections
3. Add custom ruleset, navigate to path where php-linters repository 
is cloned and choose the `phpmd.ruleset.xml`
4. Go to the Languages & Frameworks -> PHP -> Quality Tools
5. In field Mess Detector choose `configuration`
6. Navigate to path where php-liters repository is cloned and choose the `vendor/bin/phpmd` file
7. Set the tool process timeout to 15 sec

PHPCS:

Configure it in your phpstorm:

1. Settings -> Editor -> Inspections -> search for codesniffer
2. Check the box on the right
3. Check file extensions: `php`
4. Show sniff name -> yes
5. Installed standard paths: point to the path were php-linters is clonded and choose: 
`vendor/escapestudios/symfony2-coding-standard/Symfony`
6. Coding standard: Custom & navigate to the path were php-linters repository is cloned and choose `phpcs.ruleset.xml`
6. Go to Languages & Frameworks -> PHP -> Quality Tools
7. Navigate to path where php-liters repository is cloned and choose the `vendor/bin/phpcs` file
8. Set the tool process timeout to 15 sec