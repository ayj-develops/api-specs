---
title: Endpoints
layout: default
---

# Endpoints 

The following API endpoints are used to programmatically create, retrieve, update, and delete Club, Post, User and Comment objects.

|                                                                                                                                                                                                                                                                                                                                        |                                                                                                                                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `/club`, refers to endpoints that deals with the club object<br> `/post`, refers to endpoints that deals with the post object<br> `/user`, refers to endpoints that deals with the user object<br> `/comment`, refers to endpoints that deals with the comment object<br> `/`, refers to the collection of endpoints from the root url | Jump to:<br>[club endpoints](#club-object)<br>[post endpoints](#post-object)<br>[user endpoints](#user-object)<br>[comment endpoints](#comment-object)<br>[interaction endpoints](#interactions) |


## Club Object

|                                                                                             |                                                                          |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| [clubs]({{ site.baseurl }}/club-endpoint/clubs)                                             | Get all clubs                                                            |
| [clubs/create]({{ site.baseurl }}/club-endpoint/clubs-create)                               | Creates a new club                                                       |
| [clubs/{id}]({{ site.baseurl }}/club-endpoint/clubs-id)                                     | Gets a club identified by the id                                         |
| [clubs/{id}/posts]({{ site.baseurl }}/club-endpoint/clubs-id-posts)                         | Get all posts with the given club's id in the post's club field          |
| [clubs/{id}/delete]({{ site.baseurl }}/club-endpoint/clubs-id-delete)                       | Deletes a club identified by the id                                      |
| [clubs/{id}/update]({{ site.baseurl }}/club-endpoint/clubs-id-update)                       | Updates the given club                                                   |
| [clubs/{id}/executives/new]({{ site.baseurl }}/club-endpoint/clubs-id-executives-new)       | Adds an executive to the given club                                      |
| [clubs/{id}/executives/delete]({{ site.baseurl }}/club-endpoint/clubs-id-executives-delete) | Deletes an executive identified by the User object id in the given club  |
| [clubs/{id}/members]({{ site.baseurl }}/club-endpoint/clubs-id-members)                     | Gets all club members                                                    |
| [clubs/{id}/members/add]({{ site.baseurl }}/club-endpoint/clubs-id-members-add)             | Adds a new club member to the given club                                 |
| [clubs/{id}/members/delete]({{ site.baseurl }}/club-endpoint/clubs-id-members-delete)       | Deletes a club member from the given club                                |
| [clubs/{id}/favourite]({{ site.baseurl }}/club-endpoint/clubs-id-favourite)                 | Adds the given club to the authenticated user's favourite club list      |
| [clubs/{id}/unfavourite]({{ site.baseurl }}/club-endpoint/clubs-id-unfavourite)             | Removes the given club from the authenticated user's favourite club list |


## Post Object

|                                                                                   |                                      |
| --------------------------------------------------------------------------------- | ------------------------------------ |
| [posts]({{ site.baseurl }}/post-endpoint/posts)                                   | Get all posts                        |
| [posts/{id}]({{ site.baseurl }}/post-endpoint/posts-id)                           | Get specific post identified by id   |
| [posts/create]({{ site.baseurl }}/post-endpoint/posts-crete)                      | Create a new post                    |
| [posts/{id}/edit]({{ site.baseurl }}/post-endpoint/posts-id-edit)                 | Edit a given post                    |
| [posts/{id}/delete]({{ site.baseurl }}/post-endpoint/posts-id-delete)             | Delete a give post                   |
| [posts/{id}/favourite]({{ site.baseurl }}/post-endpoint/posts-id-favourite)       | Favourite the given post             |
| [posts/{id}/unfavourite]({{ site.baseurl }}/post-endpoint/posts-id-unfavourite)   | Unfavourite the given post           |
| [posts/{id}/like]({{ site.baseurl }}/post-endpoint/posts-id-like)                 | Like the given post                  |
| [posts/{id}/dislike]({{ site.baseurl }}/post-endpoint/posts-id-dislike)           | Dislike the given post               |
| [posts/{id}/comments]({{ site.baseurl }}/post-endpoint/posts-id-comments)         | Get all comments from a given post   |
| [posts/{id}/comments/add]({{ site.baseurl }}/post-endpoint/posts-id-comments-add) | Create a new comment on a given post |


## User Object

|                                                                          |                                                                            |
| ------------------------------------------------------------------------ | -------------------------------------------------------------------------- |
| [users]({{ site.baseurl }}/user-endpoint/users)                          | Gets all users                                                             |
| [users/create]({{ site.baseurl }}/user-endpoint/users-create)            | Creates a new user                                                         |
| [users/user]({{ site.baseurl }}/user-endpoint/users-user)                | Get the current authenticated user's data                                  |
| [users/delete]({{ site.baseurl }}/user-endpoint/users-delete)            | Deletes the current authenticated user                                     |
| [users/comments]({{ site.baseurl }}/user-endpoint/users-comments)        | Gets the current authenticated user's comments                             |
| [users/favourites]({{ site.baseurl }}/user-endpoint/users-id-favourites) | Gets the current authenticated user's favourite posts or clubs, filterable |
| [users/posts]({{ site.baseurl }}/user-endpoint/users-id-posts)           | Gets the current authenticated user's posts                                |
| [users/liked]({{ site.baseurl }}/user-endpoint/users-id-liked)           | Gets the current authenticated user's liked comments                       |


## Comment Object

|                                                                                 |                                  |
| ------------------------------------------------------------------------------- | -------------------------------- |
| [comments]({{ site.baseurl }}/comment-endpoint/comments)                        | Gets all comments                |
| [comments/{id}]({{ site.baseurl }}/comments-endpoint/comments-id)               | Get a comment identified by id   |
| [comments/{id}/delete]({{ site.baseurl }}/comments-endpoint/comments-id-delete) | Delete a given comment           |
| [comments/{id}/edit]({{ site.baseurl }}/comments-endpoint/comments-id-edit)     | Update a given comment           |
| [comments/{id}/like]({{ site.baseurl }}/comments-endpoint/comments-id-like)     | Like a given comment             |
| [comments/{id}/unlike]({{ site.baseurl }}/comments-endpoint/comments-id-unlike) | Remove like from a given comment |


## Interactions

<!--
## Admin level endpoints

|                                |                                                  |
| ------------------------------ | ------------------------------------------------ |
| [admin/roles]                  | Get all roles                                    |
| [admin/roles/new]              | Create a new role with permissions               |
| [admin/roles/user/{id}/update] | Update an existing user with the following roles |

Jump to [authentication]({% link _docs/authentication.md#admin-level-endpoints %}) for admin level endpoints

 --->