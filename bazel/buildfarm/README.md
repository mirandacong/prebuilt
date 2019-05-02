This directory contains deployable jars that are built from
[bazel-buildfarm](https://github.com/bazelbuild/bazel-buildfarm).

To fully reproduce the build:

commit: 6021c94f57a455586ae948ed2bab5bb08e8307db

```bash
bazel build \
    //src/main/java/build/buildfarm:buildfarm-worker_deploy.jar \
    //src/main/java/build/buildfarm:buildfarm-server_deploy.jar

cp bazel-bin/src/main/java/build/buildfarm/buildfarm-worker_deploy.jar worker.jar
cp bazel-bin/src/main/java/build/buildfarm/buildfarm-server_deploy.jar server.jar
```
