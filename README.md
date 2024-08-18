# Display product gallery thumbnails on left side - Single product page Woocommerce - Elementor Hello Theme


/* ---------------------------------------------- */


/* Functionality: Custom thumbnail size in product image gallery
 * Date:  2021-03-10
 * Author: Rafael Azuaje
 */

/* DESKTOP */
.woocommerce .flex-control-thumbs {
    margin: 10px 0px 10px -5px !important; /* Thumbnails separation top and bottom */
    width: 100% !important; /* Controls width of thumbnails container on desktop - Horizontally */
	display: flex;

}
/* Controls thumbnails width on desktop - vertically
 * Enable this ONLY for VERTICAL display
 */ 
ol.flex-control-nav.flex-control-thumbs li {
	width: 15% !important; 
	

}
/* Enable this ONLY for HORIZONTAL display */
/* ol.flex-control-nav.flex-control-thumbs li {
	width: 18% !important; 
}
 */
/* PHONES */
@media (max-width:414px){
	ol.flex-control-nav.flex-control-thumbs li {
		width: 18% !important; /* Controls thumbnails width on mobile - Horizontally */
	}
}

/* TABLETS */
@media (min-width:568px) and (max-width:768px){
	/* Controls thumbnails container width on tablet - vertically
	 * Enable this ONLY for VERTICAL display */
	.woocommerce .flex-control-thumbs {
    	margin: 10px 0px 10px -5px !important; 
    	width: 15% !important;
	}
	/* Controls width of thumbnails container on tablet - horizontally
	 * Enable this ONLY for HORIZONTAL display */
/* 	.woocommerce .flex-control-thumbs {
    	width: 70% !important; 
	} */
	ol.flex-control-nav.flex-control-thumbs li {
		width: 90% !important; /* Controls thumbnails image width on tablet - vertically */
	}
}
@media (min-width:769px) and (max-width:1024px){
	/* Controls thumbnails container width on tablet - vertically
	 * Enable this ONLY for VERTICAL display */
	.woocommerce .flex-control-thumbs {
    	margin: 10px 0px 10px -5px !important; 
    	width: 12% !important;
	}
	/* Controls width of thumbnails container on tablet - horizontally
	 * Enable this ONLY for HORIZONTAL display */
/* 	.woocommerce .flex-control-thumbs {
    	width: 70% !important; 
	} */
	ol.flex-control-nav.flex-control-thumbs li {
		width: 100% !important; /* Controls thumbnails image width on tablet - vertically */
	}
}
.flex-control-nav.flex-control-thumbs img{
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
    
}



/* ...................................... */



/* Functionality: Product page image thumbnails on left side
 * Date:  2021-03-10
 * Author: Rafael Azuaje
 * Disable this segment if you want to display horizontally
 */
@media (min-width:568px) {
	.woocommerce .flex-control-nav { 
		position: absolute; 
		top:20px; 
		left: 0px;
	}
	.flex-control-thumbs {
		display: flex;
		flex-direction: column;
	}
}
@media (min-width:568px) and (max-width:768px){
	.woocommerce .flex-viewport {
		width: 86.5% !important;
		left: 100px !important;
	}
}
@media (min-width:769px) and (max-width:1024px){
	.woocommerce .flex-viewport {
		width: 87% !important;
		left: 95px !important;
	}
}
@media (min-width:1025px){
	.woocommerce .flex-viewport {
		width: 85% !important;
		left: 80px !important;
	}	
}
