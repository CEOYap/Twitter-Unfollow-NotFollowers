# Twitter-Unfollow-NotFollowers
Javascript for unfollowing everyone who is not following you

// 1. Go to https://twitter.com/following.
// 2 Open your web-browser console and run the following codes

#Autoscroll
setInterval(function() { window.scrollTo(0, document.body.scrollHeight); }, 2000);+

#follow
```javascript
$('.user-actions.not-following').each(function () {
    var followButton = $(this).find('.user-actions-follow-button');
        followButton.click();
});
```

#Unfollow
```javascript
$('.ProfileCard-content').each(function () {
    var status = $(this).find('.FollowStatus').text();
    var unfollowButton = $(this).find('.user-actions-follow-button');
    if (status != 'follows you') {
        unfollowButton.click();
    }
});
```
```javascript
$('.ProfileCard-content').each(function(){var status = $(this).find('.FollowStatus').text();var unfollowButton = $(this).find('.user-actions-follow-button');if(status != 'follows you'){unfollowButton.click();}});
```
