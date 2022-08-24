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
| [clubs/{id}/delete]({{ site.baseurl }}/club-endpoint/clubs-id-delete)                                        | Deletes a club identified by the id                                     |
| [clubs/{id}/update]({{ site.baseurl }}/club-endpoint/clubs-id-update)                                        | Updates the given club                                                  |
| [clubs/{id}/socials/update]({{ site.baseurl }}/club-endpoint/clubs-id-socials-update)                        | Updates the given club's socials object                                 |
| [clubs/{id}/teachers/new]({{ site.baseurl }}/club-endpoint/clubs-id-teachers-new)                            | Adds a new teacher to the given club                                    |
| [clubs/{id}/teachers/{name}/delete]({{ site.baseurl }}/club-endpoint/clubs-id-teachers-name-delete)          | Deletes a teacher identified by the teacher name in the given club      |
| [clubs/{id}/executives/new]({{ site.baseurl }}/club-endpoint/clubs-id-executives-new)                        | Adds an executive to the given club                                     |
| [clubs/{id}/executives/{exec-id}/delete]({{ site.baseurl }}/club-endpoint/clubs-id-executives-execid-delete) | Deletes an executive identified by the User object id in the given club |

## Post Object



## User Object



## Comment Object




## Interactions



