import aspose.barcode as barcode

reader = barcode.barcoderecognition.BarCodeReader("C:\\Files\\Sample_qr.jpg")

recognized_results = reader.read_bar_codes()

for x in recognized_results:
    print("Code Text: " + x.code_text)
    print("Type: " + x.code_type_name)
