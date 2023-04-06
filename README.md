# my-pachyderm
```
curl -o /tmp/pachctl.deb -L https://github.com/pachyderm/pachyderm/releases/download/v2.5.3/pachctl_2.5.3_amd64.deb && sudo dpkg -i /tmp/pachctl.deb

pachctl connect grpc://10.69.41.93:80

pachctl version
COMPONENT           VERSION
pachctl             2.5.3
pachd               2.5.3


# https://docs.pachyderm.com/latest/deploy-manage/manage/pachctl-shell/

# https://github.com/pachyderm/pachyderm/tree/master/examples/word_count

pachctl create project openCV
pachctl config update context --project openCV
pachctl config get active-context
pachctl config get context local
pachctl create repo images
pachctl list repo
 pachctl put file images@master:liberty.png -f http://imgur.com/46Q8nDz.png
pachctl list commit images
# REPO          BRANCH COMMIT                           FINISHED       SIZE     ORIGIN DESCRIPTION
pachctl list commit images
pachctl list file images@master
pachctl get file images@master:liberty.png | display
pachctl create pipeline -f https://raw.githubusercontent.com/pachyderm/pachyderm/2.5.x/examples/opencv/edges.json
k get pods -n pachyderm
pachctl list job
pachctl list pipeline
pachctl list repo
pachctl put file images@master:AT-AT.png -f http://imgur.com/8MN9Kg0.png
pachctl put file images@master:kitten.png -f http://imgur.com/g2QnNqa.png
pachctl list job
pachctl create pipeline -f https://raw.githubusercontent.com/pachyderm/pachyderm/2.5.x/examples/opencv/montage.json

```

