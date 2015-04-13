# Soggy Cupcakes

The code and content for my [personal site][soggy], which is generated by
[Jekyll] [jekyll] and hosted on [Amazon S3][s3].

## Setup

+ Install [gems][gems]: `bundle install`
+ Ensure S3 credentials are present in `.env` (excluded from source control);
[more information][s3website])

## Writing

+ Start local server for previewing: `bundle exec jekyll serve --drafts` (site
will be available at `localhost:4000`)
+ Add drafts to `_drafts`
+ Write, edit and repeat until "done"
+ Move completed posts from `_drafts` to `_posts`, using the
`YYYY-MM-DD-post-title` naming convention

## Publishing

+ Generate with better recommendations, no drafts, and no future posts: `bundle
exec jekyll build --lsi`
+ Push to S3: `bundle exec s3_website push`

[gems]: https://rubygems.org/
[jekyll]: http://jekyllrb.com/
[s3]: http://aws.amazon.com/s3/
[s3website]: https://github.com/laurilehmijoki/s3_website
[soggy]: http://soggycupcakes.com/
