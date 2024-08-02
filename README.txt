<section class="panel (size modifier) (color modifier)">
					<div class="intro (color modifier)">
						(intro content)
					</div>
					<div class="inner (inner modifiers) (color modifier)">
						(inner content)
					</div>
				</section>

				Note: The entire "intro" child element can be excluded.
				Note: You can have as many "intro" and "inner" child elements as you like.

			Modifiers

				Size

					small          Use small size.
					medium         Use medium size.
					large          Use large size.

				Color

					color0         Use background color 0 (gradient).
					color1         Use background color 1.
					color2         Use background color 2.
					color3         Use background color 3.
					color4         Use background color 4.
					color1-alt     Use background color 1 (alt).
					color2-alt     Use background color 2 (alt).
					color3-alt     Use background color 3 (alt).
					color4-alt     Use background color 4 (alt).

				Inner

					columns        Divides child elements into columns.
					aligned        When used with "columns", aligns content to top of panel.
					divided        When used with "columns", separates each column with a vertical line.

			Examples

				Here's a very basic example:

					<section class="panel medium color0">
						<div class="intro">
							<h2 class="major">Panel</h2>
							<p>Just a generic panel.</p>
						</div>
						<div class="inner">
							<p>Lorem ipsum dolor sit amet.</p>
						</div>
					</section>

				And here's a more advanced example using columns and *no* size modifier:

					<section class="panel color2">
						<div class="intro">
							<h2 class="major">Panel</h2>
							<p>Just a generic panel.</p>
						</div>
						<div class="inner columns">
							<div class="span-4">
								<p>This column is 4 units wide.</p>
							</div>
							<div class="span-3">
								<p>This column is 3 units wide.</p>
							</div>
							<div class="span-2">
								<p>This column is 2 units wide.</p>
							</div>
						</div>
					</section>

				Note: The "intro" child element already has a fixed width, so a span modifier
				isn't required.


		Panel (Banner)
		--------------

			The "Banner" variant of a regular panel.

			HTML

				<section class="panel banner (size modifier) (color modifier) (orientation modifier)">
					<div class="content (color modifier)">
						(content)
					</div>
					<div class="image (image modifiers)" data-position="(image position modifier)">
						<img src="(image URL)" alt="" />
					</div>
				</section>

			Modifiers

				Orientation

					left           Content on the left, image on the right.
					right          Content on the right, image on the left.

				Image

					filtered       Applies a gradient filter to the image.
					tinted         Applies a tint filter to the image.

				Image Position (required)

					top left       Position image in the top-left corner.
					top            Position image along the top edge.
					top right      Position image in the top-right corner.
					right          Position image along the right edge.
					bottom right   Position image in the bottom-right corner.
					bottom         Position image along the bottom edge.
					bottom left    Position image in the bottom-left corner.
					left           Position image along the left edge.
					center         Position image in the center.

			Example

				<section class="panel banner medium right">
					<div class="content color0">
						<h1>Banner</h1>
						<p>Lorem ipsum dolor sit amet.</p>
					</div>
					<div class="image" data-position="center">
						<img src="/path/to/image.jpg" alt="" />
					</div>
				</section>


		Panel (Spotlight)
		-----------------

			The "Spotlight" variant of a regular panel.

			HTML

				<section class="panel spotlight (size modifier) (orientation modifier)">
					<div class="content (span modifier)">
						(content)
					</div>
					<div class="image (image modifiers)" data-position="(image position modifier)">
						<img src="(image URL)" alt="" />
					</div>
				</section>

			Modifiers

				Orientation

					left           Content on the left.
					right          Content on the right.

				Image

					filtered       Applies a gradient filter to the image.
					tinted         Applies a tint filter to the image.

				Image Position (required)

					top left       Position image in the top-left corner.
					top            Position image along the top edge.
					top right      Position image in the top-right corner.
					right          Position image along the right edge.
					bottom right   Position image in the bottom-right corner.
					bottom         Position image along the bottom edge.
					bottom left    Position image in the bottom-left corner.
					left           Position image along the left edge.
					center         Position image in the center.

			Example

				<section class="panel spotlight large right">
					<div class="content">
						<h1>Spotlight</h1>
						<p>Lorem ipsum dolor sit amet.</p>
					</div>
					<div class="image" data-position="center">
						<img src="/path/to/image.jpg" alt="" />
					</div>
				</section>


		Gallery
		-------

			A lightbox-enabled gallery.

			HTML

				<div class="gallery">
					<a href="(full image URL)" class="image (image modifiers) (span modifier)" data-position="(image position modifier)">
						<img src="(thumbnail image URL)" alt="" />
					</a>
					<a href="(full image URL)" class="image (image modifiers) (span modifier)" data-position="(image position modifier)">
						<img src="(thumbnail image URL)" alt="" />
					</a>
					<a href="(full image URL)" class="image (image modifiers) (span modifier)" data-position="(image position modifier)">
						<img src="(thumbnail image URL)" alt="" />
					</a>
					<div class="group (span modifier)">
						<a href="(full image URL)" class="image (image modifiers) (span modifier)" data-position="(image position modifier)">
							<img src="(thumbnail image URL)" alt="" />
						</a>
						<a href="(full image URL)" class="image (image modifiers) (span modifier)" data-position="(image position modifier)">
							<img src="(thumbnail image URL)" alt="" />
						</a>
						<a href="(full image URL)" class="image (image modifiers) (span modifier)" data-position="(image position modifier)">
							<img src="(thumbnail image URL)" alt="" />
						</a>
						<a href="(full image URL)" class="image (image modifiers) (span modifier)" data-position="(image position modifier)">
							<img src="(thumbnail image URL)" alt="" />
						</a>
						...
					</div>
					...
				</div>

				Note: The "group" element creates a dual-row group of images. Images inside this group will
				automatically wrap to the next row when they exceed its width (as defined by its span modifier).
				You can have as many groups in a gallery as you like.

			Modifiers

				Image

					filtered       Applies a gradient filter to the image.
					tinted         Applies a tint filter to the image.

				Image Position (required)

					top left       Position image in the top-left corner.
					top            Position image along the top edge.
					top right      Position image in the top-right corner.
					right          Position image along the right edge.
					bottom right   Position image in the bottom-right corner.
					bottom         Position image along the bottom edge.
					bottom left    Position image in the bottom-left corner.
					left           Position image along the left edge.
					center         Position image in the center.

			Example

				<div class="gallery">
					<a href="/images/thumbnails/01.jpg" class="image filtered span-2" data-position="center">
						<img src="/images/fulls/01.jpg" alt="" />
					</a>
					<a href="/images/thumbnails/02.jpg" class="image filtered span-4" data-position="center">
						<img src="/images/fulls/02.jpg" alt="" />
					</a>
					<div class="group span-4">
						<a href="/images/thumbnails/03.jpg" class="image filtered span-2" data-position="center">
							<img src="/images/fulls/03.jpg" alt="" />
						</a>
						<a href="/images/thumbnails/04.jpg" class="image filtered span-2" data-position="center">
							<img src="/images/fulls/04.jpg" alt="" />
						</a>
						<a href="/images/thumbnails/05.jpg" class="image filtered span-2" data-position="center">
							<img src="/images/fulls/05.jpg" alt="" />
						</a>
						<a href="/images/thumbnails/06.jpg" class="image filtered span-2" data-position="center">
							<img src="/images/fulls/06.jpg" alt="" />
						</a>
					</div>
				</div>


Credits:

	Demo Images:
		Unsplash (unsplash.com)

	Icons:
		Font Awesome (fontawesome.io)

	Other:
		jQuery (jquery.com)
		normalizeWheel (@miorel + @pieterv of Facebook)
		Responsive Tools (github.com/ajlkn/responsive-tools)
