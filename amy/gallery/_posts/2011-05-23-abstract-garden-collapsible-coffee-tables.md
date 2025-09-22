---
id: 134
title: 'Abstract Garden Collapsible Coffee Tables'
date: '2011-05-23T01:59:28+00:00'
author: 'Amy Alley'
layout: post
image: /wp-content/uploads/2011/05/abstractgardenboth.jpg
categories:
    - Gallery
---

Simple “Abstract Garden Design” Collapsible Coffee Tables.

<div class="gallery" markdown=1>

[ ![Abstract Garden Collapsable Coffee Tables](/wp-content/uploads/2011/05/abstractgardenboth-50x50.jpg "Abstract Garden Collapsable Coffee Tables") ](/wp-content/uploads/2011/05/abstractgardenboth-400x300.jpg "Abstract Garden Collapsable Coffee Tables")
</div>

<div class="caption"><div class="image-caption">Abstract Garden Collapsable Coffee Tables
[ ![Abstract Garden Collapsable Coffee Tables](/wp-content/uploads/2011/05/abstractgardenga-50x50.jpg "Abstract Garden Collapsable Coffee Tables") ](/wp-content/uploads/2011/05/abstractgardenga-400x300.jpg "Abstract Garden Collapsable Coffee Tables")<div class="caption"><div class="image-caption">Abstract Garden Collapsable Coffee Tables
- [ ![Abstract Garden Collapsable Coffee Tables](/wp-content/uploads/2011/05/abstractgardengside-50x50.jpg "Abstract Garden Collapsable Coffee Tables") ](/wp-content/uploads/2011/05/abstractgardengside-400x300.jpg "Abstract Garden Collapsable Coffee Tables")<div class="caption"><div class="image-caption">Abstract Garden Collapsable Coffee Tables
- [ ![Abstract Garden Collapsable Coffee Tables](/wp-content/uploads/2011/05/abstractgardenoa-50x50.jpg "Abstract Garden Collapsable Coffee Tables") ](/wp-content/uploads/2011/05/abstractgardenoa-400x300.jpg "Abstract Garden Collapsable Coffee Tables")<div class="caption"><div class="image-caption">Abstract Garden Collapsable Coffee Tables
- [ ![Abstract Garden Collapsable Coffee Tables](/wp-content/uploads/2011/05/abstractgardenot-50x50.jpg "Abstract Garden Collapsable Coffee Tables") ](/wp-content/uploads/2011/05/abstractgardenot-400x300.jpg "Abstract Garden Collapsable Coffee Tables")<div class="caption"><div class="image-caption">Abstract Garden Collapsable Coffee Tables

<div class="photospace_clear"> [](# "Previous Page") [](# "Next Page")    <div class="gal_content"><div class="controls" id="controls_134_8"><div class="slideshow-container"><div class="loader" id="loading_134_8"><div class="slideshow" id="slideshow_134_8"><div class="caption-container" id="caption_134_8">   <div class="gallery_clear"> <script type="text/javascript">

			jQuery(document).ready(function($) {

				// We only want these styles applied when javascript is enabled
				$('.gal_content').css('display', 'block');
				$('.thumnail_col').css('width', '181px');

				// Initialize Advanced Galleriffic Gallery
				var gallery = $('#thumbs_134_8').galleriffic({
					delay:                     3500,
					numThumbs:                 9,
					preloadAhead:              9,
					enableTopPager:            0,
					enableBottomPager:         false,
					imageContainerSel:         '#slideshow_134_8',
					controlsContainerSel:      '#controls_134_8',
					captionContainerSel:       '#caption_134_8',
					loadingContainerSel:       '#loading_134_8',
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
