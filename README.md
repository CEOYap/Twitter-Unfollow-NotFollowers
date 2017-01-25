# Twitter Unfollow users not following you script
Javascript for unfollowing users who are not following you

1. Go to https://twitter.com/following.

2. Open your web-browser console and run the following codes

#Autoscroll
```javascript
setInterval(function() { window.scrollTo(0, document.body.scrollHeight); }, 2000);+
```
#Unfollow users that are not following you
```javascript
$('.ProfileCard-content').each(function(){var status = $(this).find('.FollowStatus').text();
    var unfollowButton = $(this).find('.user-actions-follow-button');
    if(status != 'follows you'){unfollowButton.click();
    }
});
```
