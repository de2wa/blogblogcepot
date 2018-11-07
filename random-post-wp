<?php function rand_posts() { 
 
$args = array(
    'post_type' => 'post',
    'orderby'   => 'rand',
    'posts_per_page' => 1, 
    );
 
$the_query = new WP_Query( $args );
 
if ( $the_query->have_posts() ) {
 
//$string .= '<ul>';
    while ( $the_query->have_posts() ) {
        $the_query->the_post();
        $string =get_permalink();
    }
    //$string .= '</ul>';
    wp_reset_postdata();
} else {
 
//$string .= 'no posts found';
}
 
return $string; 
} 
 //echo 'rand' .rand_posts();
?>
