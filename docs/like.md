
# Like

`Like` handler class.

## API

### Like(post-id, site-id, WPCOM);

Create a new `Like` instance giving `post-id`, `site-id` and `WPCOM` instance.

```js
var like = Like('<post-id>', '<site-id>', WPCOM);
```

### Like#state(fn)

`Like#mine` alias.

### Like#mine(fn)

Get your Like status for a Post

```js
wpcom
.sites('blog.wordpress.com')
.post(342)
.like()
.mine(function(err, data){
  // like `data` object
});
```

### Like#add(fn)

Like the post

```js
wpcom
.sites('blog.wordpress.com')
.post(342)
.like()
.add(function(err, data){
  // I like this 342 post
});
```