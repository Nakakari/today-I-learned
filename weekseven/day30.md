```
jsx
const express = require('express');
const router = express.Router();

const login = require('./login');
const posts = require('./posts');
const signup = require('./signup');
const likes = require('./likes');
const comments = require('./comments');

router.use('./login', login);
router.use('./posts', posts);
router.use('./signup', signup);
router.use('./likes', likes);
router.use('./comments', comments);

module.exports = router;
```

