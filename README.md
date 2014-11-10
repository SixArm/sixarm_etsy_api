# SixArm.com » Etsy » <br>
API tools and examples

To get a shop:

    shop_id=FooBar
    api_key=s8pzp4l9gzu5nrrzubz31coq
    curl "https://openapi.etsy.com/v2/shops/$shop_id?method=GET&api_key=$api_key"

To get listings:

    curl "https://openapi.etsy.com/v2/shops/$shop_id/listings/active?method=GET&api_key=$api_key&fields=title,url&limit=100"

To get listings with main image:

    curl "https://openapi.etsy.com/v2/shops/$shop_id/listings/active?method=GET&api_key=$api_key&fields=title,url&limit=100&includes=MainImage"
