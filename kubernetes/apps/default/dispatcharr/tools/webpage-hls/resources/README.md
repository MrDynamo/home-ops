# Webpage to HLS

## Information

Can be used to serve static ws4kp weather channels to Dispatcharr. Alternatively, can be used to service any URL as well.

## Stream Endpoint

### Channel URLs

#### Default URL (1920x1080, 15 fps)

```
http://webpage-hls.default.svc:3000/stream?url=<ENCODED_URL>
```

#### 720p URL (1 fps)

##### Landscape (1280x720)

```
http://webpage-hls.default.svc:3000/stream?fps=1&width=1280&height=720&url=
```

##### Portrait (720x1280)

```
http://webpage-hls.default.svc:3000/stream?fps=1&width=720&height=1280&url=
```

#### 4k URL Landscape (1 fps)

##### Landscape (3840x2160)

```
http://webpage-hls.default.svc:3000/stream?fps=1&width=3840&height=2160&url=
```

##### Portait (2160x3840)

```
http://webpage-hls.default.svc:3000/stream?fps=1&width=2160&height=3840&url=
```

### Grafana

Cluster URL:
```
http://grafana-service.observability.svc.cluster.local:3000/
```

Encoded Cluster URL:
```
http%3A%2F%2Fgrafana-service.observability.svc.cluster.local%3A3000%2Fd%2F
```

1. Load dashboard in browser.
2. Set TZ manually and all relevant settings.
3. Copy URL beginning with `/d/`.
4. Add `&kiosk` to the end.
5. Encode into URL format.
6. Add to base channel URL after `url=`.
7. Create new stream in Dispatcharr with built URL.
8. Create channel from stream and set profile to `Proxy`.
