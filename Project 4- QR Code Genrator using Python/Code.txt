import qrcode
url = input("Enter your link: ")
filename = input("Filename you want to save it as: ")
if not (filename.endswith(".jpg")):
    filename = filename + ".jpg"

img = qrcode.make(url)
img.save(filename)
