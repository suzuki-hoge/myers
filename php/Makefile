build:
	docker build -t myers-triangle:php .

init:
	docker run -v $(CURDIR):/opt/project -w /opt/project --name myers-triangle-php --rm -it myers-triangle:php composer install

bash:
	docker run -v $(CURDIR):/opt/project -w /opt/project --name myers-triangle-php --rm -it myers-triangle:php bash

php:
	docker run -v $(CURDIR):/opt/project -w /opt/project --name myers-triangle-php --rm -it myers-triangle:php vendor/bin/psysh

main:
	docker run -v $(CURDIR):/opt/project -w /opt/project --name myers-triangle-php --rm -it myers-triangle:php php src/main.php ${args}

test:
	docker run -v $(CURDIR):/opt/project -w /opt/project --name myers-triangle-php --rm -it myers-triangle:php vendor/bin/phpunit tests

