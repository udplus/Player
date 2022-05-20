# Just (Video) Player 


## updateLoading
    app/src/main/java/com/brouken/player/PlayerActivity.java
        updateLoading

```java

    private void updateLoading(final boolean enableLoading) {
        if (enableLoading) {
            exoPlayPause.setVisibility(View.GONE);
            loadingProgressBar.setVisibility(View.VISIBLE);
        } else {
            loadingProgressBar.setVisibility(View.GONE);
            exoPlayPause.setVisibility(View.VISIBLE);
            if (focusPlay) {
                focusPlay = false;
                exoPlayPause.requestFocus();
            }
        }
    }


```

    updateLoading(true);
        initializePlayer()

    updateLoading(false);
        onPlaybackStateChanged
        onPlayerErro