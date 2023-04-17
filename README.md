# current-year-wordpress
create a shortcode for displaying the current year in the copyright notice
To create a shortcode for displaying the current year in the copyright notice, you can add a custom function to your theme's functions.php file. If you're using a child theme, add it to the child theme's functions.php file. Here's an example of how to create a shortcode called [current_year]:

Open your theme's functions.php file or your child theme's functions.php file.

Add code see shortcode

// Create a shortcode for displaying the current year

In this example, the current_year_shortcode() function returns the current year using the PHP date() function. The add_shortcode() function creates a new shortcode called [current_year] that's linked to the current_year_shortcode() function.

Save your functions.php file.
Now you can use the [current_year] shortcode in your WordPress posts, pages, and text widgets. If you want to use this shortcode in your theme's PHP files, you can use the do_shortcode() function, like this:

<footer>
    <p>&copy; <?php echo do_shortcode('[current_year]'); ?> Your Website Name. All rights reserved.</p>
</footer>

