"# Sarcasm-Detection"


Nhóm bao gồm:
Trần Doãn Thuyên 18521479

Link to notebook:
https://colab.research.google.com/drive/1mSmOgXrD3HioNgDJyJEdqtjxgS4haLTX?authuser=1#scrollTo=bEsb3jIXvy5F

Get Embedding Vectors matrix from:
https://drive.google.com/file/d/1-hXkwyjks0DbO2V2mfhbH9bUibnITc99/view?usp=sharing

Get Model from:
https://drive.google.com/file/d/1-piNc-MmD8wNly1U9uCRU8jn8h9rZ5or/view?usp=sharing

Get Model weights:
https://drive.google.com/file/d/1-fxifTRzrmU7Uw9eaWzRPYvn-BUHJTmY/view?usp=sharing

Get Tokenizer:
https://drive.google.com/file/d/1-sltCi9nCSQmA-xaBPutq6Yfl6YONC_H/view?usp=sharing <-

The onion headlines:
https://drive.google.com/file/d/1-XWzpmvReeTzhGhthuyVTUOKWGWJGdXZ/view?usp=sharing


### Using drive-link:
	from pydrive.auth import GoogleAuth
	from pydrive.drive import GoogleDrive
	auth.authenticate_user()
	gauth = GoogleAuth()
	gauth.credentials = GoogleCredentials.get_application_default()
	drive = GoogleDrive(gauth)
	file_id = "YOUR_FILE_ID"
	# For example: "1-sltCi9nCSQmA-xaBPutq6Yfl6YONC_H" id of Tokenizer file
	downloaded = drive.CreateFile({'id': file_id})
	downloaded.GetContentFile(os.path.join(data_dir, 'file_name.zip'))