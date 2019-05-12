# lumenTwig
lumen support twig template

## install
composer require hofa/lumen-twig

## bootsrap/app.php
$app->register(LumenTwig\TwigServiceProvider::class);

## uses
view('tests/index.twig', ['a' => 1]);  
touch resource/view/tests/index.twig

## twig global variable
{{ reqeust.input('query', 1)}}  
{{ app('hash').make('a123456')}}  
{{ session...}}
{{ url...}}
{{ auth...}}