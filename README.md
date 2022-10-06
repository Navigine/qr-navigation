# Qr navigation

This is web application for providing building routes functionality using Navigine system

## Usage

[Example of website with zoom to POI is here](https://ips.navigine.com/utils/paths?location=150&floor=194&venue=1922&hash=D8CA-9260-68D1-0494) <br>
[Example of website without zoom to POI is here](https://ips.navigine.com/utils/paths?location=150&floor=194&hash=D8CA-9260-68D1-0494)

## How to
1) Register and walk thow Navigine setup - create location, add routes and venues (POE) on map, then generate url for QR navigation by clicking on venue in navigine map and scaning QR code
2) Use it!
3) Also you can add it to your web page by iframe (exaple in repo)

### iframe code example without zoom to venue
```
<!DOCTYPE html>
<html>
<body>
    <iframe style="width: 50vw; height: 50vh;" src="https://ips.navigine.com/utils/paths?location=XXX&floor=XXX&&hash=XXXX-XXXX-XXXX" title="description"></iframe>
</body>
</html>
```

Instead of XXX use navigine's data

### iframe code example with zoom to venue
```
<!DOCTYPE html>
<html>
<body>
    <iframe style="width: 50vw; height: 50vh;" src="https://ips.navigine.com/utils/paths?location=XXX&venue=XXXfloor=XXX&&hash=XXXX-XXXX-XXXX" title="description"></iframe>
</body>
</html>
```

### url args
1) The main url ```https://ips.navigine.com/utils/paths``` 
2) location - location id in navigine system
3) floor - floor id in navigine system
4) hash - user id in navigine system
5) \*venue - optional - id of venue (POE) - map will be zoomed to venue(POE) if you'll provide this arg  

## Website features
1) Routing by clicking on map from and/or any point on map 
2) Routing from and/or to Venue (POE) on map by selecting it in selector





