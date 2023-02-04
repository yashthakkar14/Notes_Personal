### Scraper Creation
- Features to Extract
	- [x] Product Title. (span id - goodsName)
	- [x] Category. (p class - view__info-summary)
	- [x] Price. (strong class=view__info-price) (Need to review)
	- [x] Product URL.  (content = response.xpath('//meta\[@property="example"]/@content').get())
	- [x] Color. (div class = "view__table-color")
	- [x] Material. (li class = "view__detail-info-txt"\[1\])
	- [x] Rating. (dl class = "view__table-row--top-pull"/dd/last span) (last span using css selector or -1 in python).
	- [x] Number of reviews. (dl class = "view__table-row--top-pull"/a class="underline-btn")
	- [x] Model No. (p class = "view__info-style")
	- [x] Size : Pipe separated (|). (ul id = "sbOptions_25318496/li/a")
	- [x] Image URL (image class = "zoom" first image.)

### Existing Scraper Testing
- [x] Asics Scraper
- [x] Puma Scraper

### Doubts
- Price, MRP same. Need to include to the unit for the price or not?