<p align="center">
    <img src="https://github.com/octobercms/october/blob/develop/themes/demo/assets/images/october.png?raw=true" alt="October" width="25%" height="25%" />
</p>

[October](https://octobercms.com) is a Content Management System (CMS) and web platform whose sole purpose is to make your development workflow simple again. It was born out of frustration with existing systems. We feel building websites has become a convoluted and confusing process that leaves developers unsatisfied. We want to turn you around to the simpler side and get back to basics.

October's mission is to show the world that web development is not rocket science.

![Stable Build](https://github.com/octobercms/october/workflows/Tests/badge.svg?branch=1.1)
[![License](https://poser.pugx.org/october/october/license.svg)](https://packagist.org/packages/october/october)

## Installing October

Instructions on how to install October can be found at the [installation guide](https://octobercms.com/docs/setup/installation).

### Quick Start Installation

If you have composer installed, run this in your terminal to install October CMS from command line. This will place the files in a directory named **myoctober**.

    composer create-project october/october myoctober

If you plan on using a database, run this command inside the application directory.

    php artisan october:install

## Learning October

The best place to learn October is by [reading the documentation](https://octobercms.com/docs), [watching some screencasts](https://octobercms.com/support/topic/screencast) or [following some tutorials](https://octobercms.com/support/articles/tutorials).

You may also watch these introductory videos for [beginners](https://vimeo.com/79963873) and [advanced users](https://vimeo.com/172202661).

## Development Team

October was created by [Alexey Bobkov](https://www.linkedin.com/in/alexey-bobkov-232ba02b/) and [Samuel Georges](https://www.linkedin.com/in/samuel-georges-0a964131/), who both continue to develop the platform.

## Foundation library

The CMS uses [Laravel](https://laravel.com) as a foundation PHP framework.

## Contact

You can communicate with us using the following mediums:

* [Follow us on Twitter](https://twitter.com/octobercms) for announcements and updates.
* [Follow us on Facebook](https://facebook.com/octobercms) for announcements and updates.
* [Join the Official Forum](https://octobercms.com/forum) to engage with the community.
* [Join us on Discord](https://octobercms.com/chat) to chat with us.

### Premium Support

October CMS can provide premium support for a monthly fee. Find out more via the [Premium Support Program](https://octobercms.com/premium-support).

## Contributing

Before sending a Pull Request, be sure to review the [Contributing Guidelines](.github/CONTRIBUTING.md) first. We are currently operating on a smaller staff and it may take some time to reach your issue. For priority issues, consider purchasing a [premium support plan](https://octobercms.com/premium-support).

### Coding standards

Please follow the following guides and code standards:

* [PSR 4 Autoloader](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md)
* [PSR 2 Coding Style Guide](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md)
* [PSR 1 Coding Standards](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md)

### Code of Conduct

In order to ensure that the October CMS community is welcoming to all, please review and abide by the [Code of Conduct](CODE_OF_CONDUCT.md).

## License

The October CMS platform is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Security Vulnerabilities

Please review [our security policy](https://github.com/octobercms/october/security/policy) on how to report security vulnerabilities.


## Ajustes
```
	git clone git@github.com:pwerder/october1.git

	docker-compose up -d
	
	docker exec -it october1_app_1 /bin/bash
	
	composer install
	
	#Cria arquivo .env com as configurações
	php artisan october:env

	php artisan key:generate
	
	php artisan october:up
	
	chmod o+w ./storage/ -R
	
	nano /etc/apache2/apache2.conf

	#De: 
		<Directory /var/www/>
			...
			AllowOverride None
			...
		</Directory>
	#Para:
		<Directory /var/www/>
			...
			AllowOverride All
			...
		</Directory>

	a2enmod rewrite

	service apache2 restart
	
```