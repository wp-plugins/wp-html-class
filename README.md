=== Wp Html Class ===
Contributors: Maickon Rangel
Tags: html, php, tag
Requires at least: 4.1.1
Tested up to: 3.4
Stable tag: 4.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

A simple PHP class to work with PHP code instead of HTML in your projects.

== Description ==

A simple PHP class to work with PHP code instead of HTML in your projects. Once installed, simply use the object $ wp_tag to manipulate HTML elements.

With this plugin you no longer use HTML code in your projects and starts to use a $ wp_tag object that will refer to any tag.

For those who do not like to mix HTML with PHP code in your projects, this plugin offers of help.


== Installation ==

1. Unzip `wp-html-class.zip` inside the `/wp-content/plugins/` directory (or install via the built-in WordPress plugin installer)
1. Activate the plugin through the 'Plugins' admin menu in WordPress
1. Create an instance of class Class WpHtml `$ wp tag = new Wp Html Class ();` within your PHP files and start using HTML tags with PHP code.

== Screenshots ==

1. This screen shot description corresponds to screenshot-1.(png|jpg|jpeg|gif). Note that the screenshot is taken from
the /assets directory or the directory that contains the stable readme.txt (tags or trunk). Screenshots in the /assets 
directory take precedence. For example, `/assets/screenshot-1.png` would win over `/tags/4.3/screenshot-1.png` 
(or jpg, jpeg, gif).
2. This is the second screen shot


== Wp-Html-Class ==
Uma simples classe PHP para se trabalhar com códigos PHP ao invés de HTML em seus projetos. Após instalado, basta utilizar o objeto $wp_tag para manipular os elementos HTML.

`
/**
 * Exemplo de uso da classe WpHtmlClass.
 * A abertura da tag é feita com um método. Este método possui somente um parametro.
 * Este parâmetro é uma String.
 * 
 */
	<?php
	    $wp_tag->div('class="x" id="y"'); //Abre uma tag DIV com classe e id 
	    $wp_tag->div; // fecha a tag DIV

	    $wp_tag->hr(); //criar uma linha

	    $wp_tag->img('src="img/image.png"'); //cria uma imagem

	    $wp_tag->h1();
	        $wp_tag->wp_print('Hello World'); //inprime uma string

	        //wp_print() aceita um segundo parametro que por padrão é null
	        //ele pode ser "decode" ou "encode"
	        $wp_tag->wp_print('Hello World','decode'); 
	    $wp_tag->h1;
	?>
`

A idéia principal é tornar o código mais claro, sem precisar estar misturando elementos HTML com PHP.

-----------------------------------------------------------------------------------------------------
=English=
A simple PHP class to work with PHP code instead of HTML in your projects. Once installed, simply use the object $ wp_tag to manipulate HTML elements. ex:

`
/**
 * Example using the Wp Html Class class.
 * The opening of the tag is performed with a method. This method has only one parameter.
 * This parameter is a String.
 * 
 */

	<?php
	    $wp_tag->div('class="x" id="y"'); //Opens a DIV tag with class and id
	    $wp_tag->div; //closes the DIV tag

	    $wp_tag->hr(); //create a line

	    $wp_tag->img('src="img/image.png"'); //create a image

	    $wp_tag->h1();
	        $wp_tag->wp_print('Hello World'); //print a string

	        //print_wp () accepts a second parameter that by default is null
	        //it can be "decode" or "encode"
	        $wp_tag->wp_print('Hello World','decode'); 
	    $wp_tag->h1;
	?>
The main idea is to make the code clearer, without being mixing HTML elements with PHP.
`
