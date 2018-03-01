# Change the Woocommerce star ratings to show stars rather than theme ratings
We must show thanks to the Woo ninjas for this loving tutorial.

The default rating system that comes with WooCommerce is the stars, but we have disable this so that the rating system matched our themes. If you wold like to replace this with the WooCommerce default. Save the image below or get it from “plugins/WooCommerce/assets/images” and place it  in your themes “images” folder{star}(https://i2.wp.com/www.pootlepress.com/wp-content/uploads/2014/04/star.png)Then add the following to your custom.css (if you have child theme the style.css) :

```
.star-rating{float:right;width:80px;height:16px;background:url(images/star.png) repeat-x left 0} 
.star-rating span{background:url(images/star.png) repeat-x left -32px;height:0;padding-top:16px;overflow:hidden;float:left} 
.hreview-aggregate .star-rating{margin:10px 0 0 0} 
#review_form #respond{position:static;margin:0;width:auto;padding:0 0 0;background:transparent none;border:0} 
#review_form #respond:after{content:"";display:block;clear:both} 
#review_form #respond p{margin:0 0 10px} 
#review_form #respond .form-submit input{left:auto} 
#review_form #respond textarea{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;width:100%} 
p.stars:after{content:"";display:block;clear:both} 
p.stars span{width:80px;height:16px;position:relative;float:left;background:url(images/star.png) repeat-x left 0} 
p.stars span a{float:left;position:absolute;left:0;top:0;width:16px;height:0;padding-top:16px;overflow:hidden} 
p.stars span a:hover,p.stars span a:focus{background:url(images/star.png) repeat-x left -16px} 
p.stars span a.active{background:url(images/star.png) repeat-x left -32px} 
p.stars span a.star-1{width:16px;z-index:10} 
p.stars span a.star-2{width:32px;z-index:9} 
p.stars span a.star-3{width:48px;z-index:8} 
p.stars span a.star-4{width:64px;z-index:7} 
p.stars span a.star-5{width:80px;z-index:6}
```
