---
id: 446
title: 'Recreated Heirloom Crib'
date: '2011-06-10T11:59:56-06:00'
author: 'David Alley'
layout: post
guid: 'http://www.alleycraft.com/wood/?p=446'
permalink: /recreated-heirloom-crib/
image: /wp-content/uploads/2011/06/Crib09.jpg
categories:
    - Gallery
---

<div class="gallery_clear"></div><div class="photospace" id="gallery_446_5"> <div class="thumbs_wrap2"><div class="thumbs_wrap"><div class="thumnail_col " id="thumbs_446_5">- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib01-50x37.jpg "Crib01") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib01-400x300.jpg "Crib01")<div class="caption"> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib02-50x38.jpg "Crib02") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib02-400x310.jpg "Crib02")<div class="caption"> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib04-50x40.jpg "Crib04") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib04-400x324.jpg "Crib04")<div class="caption"> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib05-37x50.jpg "Crib05") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib05.jpg "Crib05")<div class="caption"> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib08-37x50.jpg "Crib08") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib08.jpg "Crib08")<div class="caption"> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib09-50x40.jpg "Crib09") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib09-400x326.jpg "Crib09")<div class="caption"> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib10-47x50.jpg "Crib10") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib10.jpg "Crib10")<div class="caption"> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib17-50x37.jpg "Crib17") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib17-400x300.jpg "Crib17")<div class="caption"><div class="image-caption">Our neighbor Rinah demonstrates</div> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib22-50x37.jpg "Crib22") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib22-400x300.jpg "Crib22")<div class="caption"><div class="image-caption">Don't drop Teddy.</div> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib25-50x37.jpg "Crib25") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib25-400x300.jpg "Crib25")<div class="caption"><div class="image-caption">Can I have this dance?</div> </div>
- [ ![](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib27-50x37.jpg "Crib27") ](https://www.alleycraft.com/wood/wp-content/uploads/2011/06/Crib27-400x300.jpg "Crib27")<div class="caption"><div class="image-caption">Custom shipping box.</div> </div>



			jQuery(document).ready(function($) {

				// We only want these styles applied when javascript is enabled
				$('.gal_content').css('display', 'block');
				$('.thumnail_col').css('width', '190px');

				// Initialize Advanced Galleriffic Gallery
				var gallery = $('#thumbs_446_5').galleriffic({
					delay:                     3500,
					numThumbs:                 18,
					preloadAhead:              18,
					enableTopPager:            0,
					enableBottomPager:         false,
					imageContainerSel:         '#slideshow_446_5',
					controlsContainerSel:      '#controls_446_5',
					captionContainerSel:       '#caption_446_5',
					loadingContainerSel:       '#loading_446_5',
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
