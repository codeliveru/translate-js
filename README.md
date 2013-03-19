# Usage
## Declare translations

```javascript
var messages = {
    en_US = {
        success: {
            comment: {
                add: 'Your comment has been added successfully',
                remove: 'Your comment has been removed',
                edit: 'Your comment has been updated'
            },
            feedback: {
                send: 'Your feedback successfully send to administrator',
                receive: 'New response for your feedback has been received'
            }
        }
    }
};
```

## Setup the default language

```javascript
var settings = {
    lang: 'en_US'
};
```

## Translate

With default language:

```javascript
var translated = tr('success:comment:add');
```

With custom language:

```javascript
var translated = tr('success:comment:edit', 'ru_RU');
```
