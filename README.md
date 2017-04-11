# SCSS block-grid mixin for Twitter Bootstrap

This is a Foundation style SCSS block-grid mixin for Twitter Bootstrap 3, based heavily on this implementation by [NodeNerd.com](http://www.nodenerd.com/using-foundations-block-grid-mixin-within-bootstrap-css-framework-updated).

&nbsp;

## Installation

### SCSS

Save the `block-grid.scss` into your current project, and then import it either into `bootstrap.scss` or into your main SCSS file.

    @import 'block-grid';



## Usage

The simplest usage is as follows.

HTML

    <div class="block-grid">
    	<div class="block-grid-item>
        	...
    	</div>
    	<div class="block-grid-item>
        	...
    	</div>
    	...
    </div>

SCSS

    .block-grid {
    	@include make-block-grid(1,2,4,6);
    }
    
&nbsp;

Otherwise, you could use the more verbose SCSS.

	.block-grid {
		@include make-block-grid-container;
		
		.block-grid-item {
			@include make-xs-block-grid(1);
			@include make-sm-block-grid(2);
			@include make-md-block-grid(4);
			@include make-lg-block-grid(6);
		}
	}

---

*The author is neither affiliated with nor endorsed by Twitter.*
