# Macdom Bundle
[Macdom HTML Preprocessor](https://github.com/Machy8/Macdom) bundle for Symfony Framework.

## Installation
````
composer require machy8/macdom-bundle
````

## Usage
````PHP
use Macdom\Engine;

/**
 * @Route("/", name="homepage")
 */
public function homepage(Engine $macdom) : Response
{
    return new Response($macdom->compile('h1 Hello World!'));
}
````

