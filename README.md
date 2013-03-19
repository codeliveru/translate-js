# Demo

[View demo](example.html)


### Define translations

```javascript
var settings = {}, messages = {};
settings.lang = 'en_US';

/* English translations */
messages.en_US = {
    success: {
        comment: {
            add: 'Your comment has been added successfully',
            remove: 'Your comment has been removed',
            edit: 'Your comment has been updated'
        },
        feedback: {
            send: 'Your feedback successfully send to administrator',
            receive: 'New response for your feedback has been received'
        },
    },
    error: {
        comment: {
            add: 'Cannot to add your commend',
            remove: 'Cannot delete your comment',
            edit: 'Cannot update your comment',
        },
        feedback: {
            send: 'Cannot to send your feedback',
            receive: 'Cannot to read the received message',
        }
    },
    action: {
        hide: 'Hide',
        show: 'Show'
    }
};
/* End English translations */
```

### Translate

With default language:

```javascript
var translated = tr('success:comment:add');
```

With custom language:

```javascript
var translated = tr('success:comment:edit', 'ru_RU');
```
