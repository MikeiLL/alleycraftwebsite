---
id: 57
title: 'Faery Table'
date: '2011-05-21T21:11:55+00:00'
author: 'Amy Alley'
layout: post
image: /wp-content/uploads/2011/05/FaeryTableTop.jpg
categories:
    - Gallery
---

This Pink and Periwinkle Faery Table brings magic to your child’s play area.

<div class="gallery_clear"></div><div class="photospace" id="gallery_57_2"> <div class="thumbs_wrap2"><div class="thumbs_wrap"><div class="thumnail_col " id="thumbs_57_2">- [ ![Faery Table](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableTop-50x50.jpg "Faery Table") ](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableTop-400x300.jpg "Faery Table")<div class="caption"><div class="image-caption">Faery Table</div><div class="image-desc">Faery Table</div> </div>
- [ ![Faery Table](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableFront-50x50.jpg "Faery Table") ](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableFront.jpg "Faery Table")<div class="caption"><div class="image-caption">Faery Table</div><div class="image-desc">Faery Table</div> </div>
- [ ![Faery Table](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableFaery-50x50.jpg "Faery Table") ](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableFaery.jpg "Faery Table")<div class="caption"><div class="image-caption">Faery Table</div><div class="image-desc">Faery Table</div> </div>
- [ ![Faery Table](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableBottom-50x50.jpg "Faery Table") ](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableBottom-400x300.jpg "Faery Table")<div class="caption"><div class="image-caption">Faery Table</div><div class="image-desc">Faery Table</div> </div>
- [ ![Faery Table](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableAngle-50x50.jpg "Faery Table") ](https://www.alleycraft.com/craft/wp-content/uploads/2011/05/FaeryTableAngle.jpg "Faery Table")<div class="caption"><div class="image-caption">Faery Table</div> </div>

<div class="photospace_clear"></div> [](# "Previous Page") [](# "Next Page") </div> </div> </div> <div class="gal_content"><div class="controls" id="controls_57_2"></div><div class="slideshow-container"><div class="loader" id="loading_57_2"></div><div class="slideshow" id="slideshow_57_2"></div><div class="caption-container" id="caption_57_2"></div> </div> </div> </div><div class="gallery_clear"></div> <script type="text/javascript">

			jQuery(document).ready(function($) {

				// We only want these styles applied when javascript is enabled
				$('.gal_content').css('display', 'block');
				$('.thumnail_col').css('width', '181px');

				// Initialize Advanced Galleriffic Gallery
				var gallery = $('#thumbs_57_2').galleriffic({
					delay:                     3500,
					numThumbs:                 9,
					preloadAhead:              9,
					enableTopPager:            0,
					enableBottomPager:         false,
					imageContainerSel:         '#slideshow_57_2',
					controlsContainerSel:      '#controls_57_2',
					captionContainerSel:       '#caption_57_2',
					loadingContainerSel:       '#loading_57_2',
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
