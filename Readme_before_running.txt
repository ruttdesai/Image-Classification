1. I have not sent the folder of data images.
2. While running the code, the Step 1 will download the images automatically in 
   the system.
3. While giving the link of the images, I got an error as '403: Forbidden'. This 
   happened with few files but in some files it didn't. I couldn't find the
   solution to the problem. I am attaching the link of some images to which the 
   error didn't produce.





Links:
	https://i.insider.com/4cf65998ccd1d5ae1d130000?width=600&format=jpeg&auto=webp
	https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTGKvDQlyCamYZF4KaZd_Dx6c-IEx6YGE2V5Q&usqp=CAU
	https://cdn.mos.cms.futurecdn.net/YB6aQqKZBVjtt3PuDSkJKe.jpg
	https://static01.nyt.com/images/2020/01/28/science/09OBS-PARROTS/09TB-PARROTS-videoSixteenByNineJumbo1600.jpg





Error:
	HTTPError                                 Traceback (most recent call last)

<ipython-input-135-b172a4546fd9> in <module>()
      3 flat_data = []
      4 url = input("Enter your image url: ")
----> 5 img = imread(url)
      6 img_resized = resize(img,(100,100,3))
      7 flat_data.append(img_resized.flatten())

8 frames

/usr/lib/python3.7/urllib/request.py in http_error_default(self, req, fp, code, msg, hdrs)
    647 class HTTPDefaultErrorHandler(BaseHandler):
    648     def http_error_default(self, req, fp, code, msg, hdrs):
--> 649         raise HTTPError(req.full_url, code, msg, hdrs, fp)
    650 
    651 class HTTPRedirectHandler(BaseHandler):

HTTPError: HTTP Error 403: Forbidden

