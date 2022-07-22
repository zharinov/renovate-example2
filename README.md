# renovate-example2

reproduction repo for discussion issue renovatebot/renovate#16708

This is an example repo to reproduce the following issue:

It seems like Renovate does not grab the latest version for packages `grpc/grpc` (github repo) and I am not sure why.

I tried different ways to grab the package (either via `github-releases` or `github-tags` datasources) but as you can see from the open PR
it's trying to update the package version to 1.47/1.47.1 even though the latest release is v1.48.0.
For comparison, I also set package grpc/grpc-java which does grab the latest version correctly.

I tried to see if there are any differences between the latest releases in grpc/grpc and grpc/grpc-java but did not find any.

https://github.com/grpc/grpc/releases

https://github.com/grpc/grpc-java/releases
