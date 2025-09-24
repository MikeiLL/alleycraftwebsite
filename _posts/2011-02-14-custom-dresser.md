---
id: 328
title: 'Custom Sink Cabinet'
date: '2011-02-14T16:32:23-06:00'
author: 'David Alley'
layout: post
guid: 'http://www.alleycraft.com/wood/?p=328'
permalink: /custom-dresser/
image: /wp-content/uploads/2011/02/ShopOne15.jpg
categories:
    - Gallery
---

<div class="gallery_clear"></div><div class="photospace" id="gallery_328_3"> <div class="thumbs_wrap2"><div class="thumbs_wrap"><div class="thumnail_col " id="thumbs_328_3">- [ ![design illustration sketch](/wp-content/uploads/2011/02/ShopOne15-50x37.jpg "ShopOne15") ](/wp-content/uploads/2011/02/ShopOne15-400x299.jpg "ShopOne15")<div class="caption"><div class="image-caption">The Design on Paper</div> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne20-50x37.jpg "ShopOne20") ](/wp-content/uploads/2011/02/ShopOne20-400x299.jpg "ShopOne20")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne19-50x37.jpg "ShopOne19") ](/wp-content/uploads/2011/02/ShopOne19-400x299.jpg "ShopOne19")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne18-50x37.jpg "ShopOne18") ](/wp-content/uploads/2011/02/ShopOne18-400x299.jpg "ShopOne18")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne17-50x37.jpg "ShopOne17") ](/wp-content/uploads/2011/02/ShopOne17-400x299.jpg "ShopOne17")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne16-50x37.jpg "ShopOne16") ](/wp-content/uploads/2011/02/ShopOne16-400x299.jpg "ShopOne16")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne14-50x37.jpg "ShopOne14") ](/wp-content/uploads/2011/02/ShopOne14-400x299.jpg "ShopOne14")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne13-50x37.jpg "ShopOne13") ](/wp-content/uploads/2011/02/ShopOne13-400x299.jpg "ShopOne13")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne12-50x37.jpg "ShopOne12") ](/wp-content/uploads/2011/02/ShopOne12-400x299.jpg "ShopOne12")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne11-50x37.jpg "ShopOne11") ](/wp-content/uploads/2011/02/ShopOne11-400x299.jpg "ShopOne11")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne10-50x37.jpg "ShopOne10") ](/wp-content/uploads/2011/02/ShopOne10-400x299.jpg "ShopOne10")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne09-50x37.jpg "ShopOne09") ](/wp-content/uploads/2011/02/ShopOne09-400x299.jpg "ShopOne09")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne08-50x37.jpg "ShopOne08") ](/wp-content/uploads/2011/02/ShopOne08-400x299.jpg "ShopOne08")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne04-50x37.jpg "ShopOne04") ](/wp-content/uploads/2011/02/ShopOne04-400x299.jpg "ShopOne04")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne03-50x37.jpg "ShopOne03") ](/wp-content/uploads/2011/02/ShopOne03-400x299.jpg "ShopOne03")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne02-50x37.jpg "ShopOne02") ](/wp-content/uploads/2011/02/ShopOne02-400x299.jpg "ShopOne02")<div class="caption"> </div>
- [ ![](/wp-content/uploads/2011/02/ShopOne01-50x37.jpg "ShopOne01") ](/wp-content/uploads/2011/02/ShopOne01-400x299.jpg "ShopOne01")<div class="caption"> </div>



			jQuery(document).ready(function($) {

				// We only want these styles applied when javascript is enabled
				$('.gal_content').css('display', 'block');
				$('.thumnail_col').css('width', '190px');

				// Initialize Advanced Galleriffic Gallery
				var gallery = $('#thumbs_328_3').galleriffic({
					delay:                     3500,
					numThumbs:                 18,
					preloadAhead:              18,
					enableTopPager:            0,
					enableBottomPager:         false,
					imageContainerSel:         '#slideshow_328_3',
					controlsContainerSel:      '#controls_328_3',
					captionContainerSel:       '#caption_328_3',
					loadingContainerSel:       '#loading_328_3',
					renderSSControls:          true,
					renderNavControls:         true,
					playLinkText:              '',
					pauseLinkText:             '',
					prevLinkText:              '',
					nextLinkText:              '',
					nextPageLinkText:          '&rsaquo;',
					prevPageLinkText:          '&lsaquo;',
					enableHistory:              0,
					autoStart:                 	1,
					enableKeyboardNavigation:	true,
					syncTransitions:           	1,
					defaultTransitionDuration: 	300,

					onTransitionOut:           function(slide, caption, isSync, callback) {
						slide.fadeTo(this.getDefaultTransitionDuration(isSync), 0.0, callback);
						caption.fadeTo(this.getDefaultTransitionDuration(isSync), 0.0);
					},
					onTransitionIn:            function(slide, caption, isSync) {
						var duration = this.getDefaultTransitionDuration(isSync);
						slide.fadeTo(duration, 1.0);

						// Position the caption at the bottom of the image and set its opacity
						var slideImage = slide.find('img');
						caption.width(slideImage.width())
							.css({
								//'bottom' : Math.floor((slide.height() - slideImage.outerHeight()) / 2 - 40),
								'top' : slideImage.outerHeight(),
								'left' : Math.floor((slide.width() - slideImage.width()) / 2) + slideImage.outerWidth() - slideImage.width()
							})
							.fadeTo(duration, 1.0);

					},
					onPageTransitionOut:       function(callback) {
						this.hide();
						setTimeout(callback, 100); // wait a bit
					},
					onPageTransitionIn:        function() {
						var prevPageLink = this.find('a.prev').css('display', 'none');
						var nextPageLink = this.find('a.next').css('display', 'none');

						// Show appropriate next / prev page links
						if (this.displayedPage > 0)
							prevPageLink.css('display', 'block');

						var lastPage = this.getNumPages() - 1;
						if (this.displayedPage < lastPage)
							nextPageLink.css('display', 'block');

						this.fadeTo('fast', 1.0);
					}

				});



				/**************** Event handlers for custom next / prev page links **********************/

				gallery.find('a.prev').click(function(e) {
					gallery.previousPage();
					e.preventDefault();
				});

				gallery.find('a.next').click(function(e) {
					gallery.nextPage();
					e.preventDefault();
				});

			});
		</script>
