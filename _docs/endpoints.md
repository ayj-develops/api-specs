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

|                                                                                                              |                                                                         |
| ------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------- |
| [clubs]({{ site.baseurl }}/club-endpoint/clubs)                                                              | Get all clubs                                                           |
| [clubs/create]({{ site.baseurl }}/club-endpoint/clubs-create)                                                | Creates a new club                                                      |
| [clubs/{id}]({{ site.baseurl }}/club-endpoint/clubs-id)                                                      | Gets a club identified by the id                                        |
| [clubs/{id}/posts]({{ site.baseurl }}/club-endpoint/clubs-id-posts)                                          | Get all posts with the given club's id in the post's club field         |
| [clubs/{id}/delete]({{ site.baseurl }}/club-endpoint/clubs-id-delete)                                        | Deletes a club identified by the id                                     |
| [clubs/{id}/update]({{ site.baseurl }}/club-endpoint/clubs-id-update)                                        | Updates the given club                                                  |
| [clubs/{id}/socials/update]({{ site.baseurl }}/club-endpoint/clubs-id-socials-update)                        | Updates the given club's socials object                                 |
| [clubs/{id}/teachers/new]({{ site.baseurl }}/club-endpoint/clubs-id-teachers-new)                            | Adds a new teacher to the given club                                    |
| [clubs/{id}/teachers/{name}/delete]({{ site.baseurl }}/club-endpoint/clubs-id-teachers-name-delete)          | Deletes a teacher identified by the teacher name in the given club      |
| [clubs/{id}/executives/new]({{ site.baseurl }}/club-endpoint/clubs-id-executives-new)                        | Adds an executive to the given club                                     |
| [clubs/{id}/executives/{exec-id}/delete]({{ site.baseurl }}/club-endpoint/clubs-id-executives-execid-delete) | Deletes an executive identified by the User object id in the given club |
| [clubs/{id}/members]({{ site.baseurl }}/club-endpoint/clubs-id-members)                                      | Gets all club members                                                   |
| [clubs/{id}/members/add]({{ site.baseurl }}/club-endpoint/clubs-id-members-add)                              | Adds a new club member to the given club                                |
| [clubs/{id}/members/delete]({{ site.baseurl }}/club-endpoint/clubs-id-members-delete)                        | Deletes a club member from the given club                               |


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

|                                                                               |                                                         |
| ----------------------------------------------------------------------------- | ------------------------------------------------------- |
| [users]({{ site.baseurl }}/user-endpoint/users)                               | Gets all users                                          |
| [users/create]({{ site.baseurl }}/user-endpoint/users-create)                 | Creates a new user                                      |
| [users/{id}]({{ site.baseurl }}/user-endpoint/users-id)                       | Gets a user identified by id                            |
| [users/{id}/delete]({{ site.baseurl }}/user-endpoint/users-id-delete)         | Deletes a user identified by id                         |
| [users/{id}/comments]({{ site.baseurl }}/user-endpoint/users-id-comments)     | Gets a given user's comments                            |
| [users/{id}/favourites]({{ site.baseurl }}/user-endpoint/users-id-favourites) | Gets a given user's favourite posts                     |
| [users/{id}/posts]({{ site.baseurl }}/user-endpoint/users-id-posts)           | Gets a given user's posts                               |
| [users/{id}/liked]({{ site.baseurl }}/user-endpoint/users-id-liked)           | Gets a given user's liked posts or comments, filterable |


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

