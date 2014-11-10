# SixArm.com » Etsy » <br> API tools and examples

Setup:

    api=https://openapi.etsy.com/v2
    api_key=s8pzp4l9gzu5nrrzubz31coq
    shop_id=FooBar

To get a shop:

    curl "$api/shops/$shop_id?method=GET&api_key=$api_key"

To get listings:

    curl "$api/shops/$shop_id/listings/active?method=GET&api_key=$api_key&fields=title,url&limit=100"

To get listings with main image:

    curl "$api/shops/$shop_id/listings/active?method=GET&api_key=$api_key&fields=title,url&limit=100&includes=MainImage"
