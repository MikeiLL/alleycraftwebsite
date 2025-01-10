---
id: 445
title: 'Anatomy of a Kitchen Renovation'
date: '2011-06-06T15:39:48-06:00'
author: 'David Alley'
layout: revision
guid: 'http://www.alleycraft.com/wood/archives/445'
permalink: /358-revision-8/
---

Removing, redesigning and rebuilding a kitchen is quite a project and this one ended up being documented from beginning to end so here it is:

<div class="gallery_clear"></div><div class="photospace" id="gallery_445_17"> <div class="thumbs_wrap2"><div class="thumbs_wrap"><div class="thumnail_col " id="thumbs_445_17"> 
<div class="photospace_clear"></div> [](# "Previous Page") [](# "Next Page") </div> </div> </div> <div class="gal_content"><div class="controls" id="controls_445_17"></div><div class="slideshow-container"><div class="loader" id="loading_445_17"></div><div class="slideshow" id="slideshow_445_17"></div><div class="caption-container" id="caption_445_17"></div> </div> </div> </div><div class="gallery_clear"></div> <script type="text/javascript">
			
			jQuery(document).ready(function($) {
				
				// We only want these styles applied when javascript is enabled
				$('.gal_content').css('display', 'block');
				$('.thumnail_col').css('width', '190px');
				
				// Initialize Advanced Galleriffic Gallery 
				var gallery = $('#thumbs_445_17').galleriffic({ 
					delay:                     3500,
					numThumbs:                 18,
					preloadAhead:              18,
					enableTopPager:            0,
					enableBottomPager:         false,
					imageContainerSel:         '#slideshow_445_17',
					controlsContainerSel:      '#controls_445_17',
					captionContainerSel:       '#caption_445_17',  
					loadingContainerSel:       '#loading_445_17',
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