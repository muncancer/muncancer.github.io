# Nätverket mot muncancer

Web pages for Nätverket mot muncancer

## How-to

### Misc site settings
[`_config.yml`](_config.yml)

### Add a page
* In [`_data/navigation.yml`](_data/navigation.yml) you find the `Main menu`.
* In [`assets/images`](assets/images) are all images.


### Add a news
Go to [`_pages/index.md`](_pages/index.md) and add the news at the top after `Most recent news`. 
Format for news: the date is in ***italic bold*** and contains the year if it is in the `index.md` file. Title of papers go in *italic*, awards go in **bold**, venues can go in italic but not necessarily. Try to also include relevant liks if possible.

### Add a member
Go to [`_pages/people.md`](_pages/people.md), depending on the new member scroll to `feature_row_professors`, `feature_row_postdocs`, `feature_row_phds` or `feature_row_masters` and add a new member. Place the profile picture under `assets/images/people`, if the picture is too big in size, please resize it / compress it. It is **important** that the format of the image is jpg (otherwise it will break the members system in the publications page) and that the filename only contains the name of the new member e.g. `alessio.jpg`. Also don't forget to update the list of members in the very top part under `excerpt`.

### Remove a member
Go to [`_pages/people.md`](_pages/people.md) and remove the member, also go to `assets/images/people` and delete their profile photo. Then put their name and former role in the Alumni section of [`_pages/people.md`](_pages/people.md). Also don't forget to update the list of members in the very top part under `excerpt`.

### Add a publication
Place the publication picture (if any) under `assets/images/publications`, if the picture is too big in size, please resize it / compress it. Go to [`_pages/index.md`](_pages/index.md) and add a new entry under `feature_row` *and* delete the last entry. Go to [`_pages/publications.md`](_pages/publications.md) and add the new entry under `feature_row`. If the list becomes very long, please consider removing the last entry from the `feature_row` and add the publication under `Older publications`. In that case, please remember to also delete the associated image under `assets/images/publications`!

New: now you can add authors from outside the lab using "other".


## Local Development (not needed thanks to [GitHub Actions](https://jekyllrb.com/docs/continuous-integration/github-actions/))

Install Jekyll: [Jekyll - Installation](https://jekyllrb.com/docs/installation/)

Fetch and update bundled gems: run `bundle`

Start the website: `bundle exec jekyll serve`
