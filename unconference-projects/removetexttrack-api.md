# `video.removeTextTrack`

## Background

Browsers have an API for working with and managing Text Tracks. Text Tracks are the way that browsers expose things like Captions and Subtitles to a developer. There are two ways to add new tracks: add a `<track>` element as a child of the video element, or use the `video.addTextTrack` API method.

These two methods are not the same. With the `<track>` element, you can remove the TextTrack by removing that `<track>` element. With `video.addTextTrack`, you cannot remove the created TextTrack.

Originally, the HTML spec had a `video.removeTextTrack` method but it was removed shortly after because it was unnecessary and it could potentially cause issues if a developer tried to remove a TextTrack that a browser was writing cues into.

## Updating the Spec

Last year, shortly after the [Demuxed](http://demuxed.com) conference, Evol created an issue on the [HTML spec](https://github.com/whatwg/html/issues/1921) to ask whether it's time to add this method back in.

The landscape as changed quite a bit since the `removeTextTrack` was removed. [Media Source Extensions (MSE)](https://en.wikipedia.org/wiki/Media_Source_Extensions) has become prevalent for playing back video on the web. Because of MSE usage, developers also need to start managing their own TextTracks so having `removeTextTrack` for programmatic removal of text tracks is important.

### Agreement

In the issue, there was consensus that it was time to add it back. However, due to low interest from browser vendors, the agreed upon course of action was to add tests to the [web platform tests](https://github.com/w3c/web-platform-tests/).

## Work at TextAV

At TextAV, we wrote some failing tests for the HTMLMediaElement component and submitted a [PR](https://github.com/w3c/web-platform-tests/pull/6594/) for the changes.

## Next Steps

The immediate next step would be to update the actual spec and iron out the small details.