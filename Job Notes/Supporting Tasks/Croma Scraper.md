- [x] Review Text
- [x] Review Description
- [x] Review Date
- [x] Review Rating
- [x] Review Upvotes (Not available)
- [x] Review Downvotes (Not available)
- [x] Verified Purchase
- [x] Review Count
- [x] Product Rating (Not Available)
- [ ] Product Title
- [x] Review ID
- [x] For each review - 1 Mongo Document.
- [x] Review sorted by latest.

#### Details Present in Reviews Response.
Feature ID
Time Tag
Site ID
proxy id
run_count not reset
try_count
is_picked
is_done
is_fail

#### Tag Update
- [ ] Is Picked
- [ ] Is Fail
- [ ] Is Done
- [ ] Add data, how many reviews present and how many scraped. How many pages present and how many scraped.

#### Changes to be Done
- [x] Change dictionary keys
- [ ] Error handling for response_data. In case the response body has no data or is not what was expected?
- [x] Error handling when fetching values from response_data. What if the key is not present
- [ ] Edge case handling for dictionary keys. What is page size is None it will throw division error.
- [ ] Output item does not have scrape date and time tag
- [ ] Use the following key structure for Reviews
```Python
    item = {
        'sku_id': request_sku_id,
        'scrape_date': request_scrape_date,
        'time_tag': request_time_tag,
        'url': request_url,
        'review_id': review_id,
        'review_url': review_url,
        'title': title,
        'text': text,
        'rating_avg': rating,
        'review_date': parsed_date,
        'original_date': original_date,
        'is_certified_buyer': is_certified_buyer,
        'downvotes': downvote_count,
        'upvotes': upvote_count,
        'page_no': request_page_no,
        'rank': request_start_rank + current_page_rank,
        'product_title': product_title,
        'product_rating_avg': rating_avg,
        'product_rating_count': rating_count,
        'product_rating_polarity': rating_pct,
        'product_review_count': review_count,
    }
```
- [ ] Process all updates after parsing. Separate blocks for parsing and updates 
- [ ] Result data updation for page 0 and other pages are coinciding. Page 1 will set pages_done_count as total pages.
- [x] Change update logic for done - Don't fetch, check and then update. Use update query.