# Podman

> காய்கள், கொள்கலன்கள் மற்றும் படங்களுக்கான எளிய மேலாண்மை கருவி.
> போட்மேன் ஒரு Docker-CLI ஒப்பிடக்கூடிய கட்டளை வரியை வழங்குகிறது. எளிமையாகச் சொன்னால்: `alias docker=podman`.
> மேலும் விவரத்திற்கு: <https://github.com/containers/podman/blob/main/commands-demo.md>.

- கொள்கலன்கள் பற்றிய தகவலை அச்சிடவும்:

`podman ps`

- அனைத்து கொள்கலன்களையும் பட்டியலிடு (இரண்டும் இயங்கும் மற்றும் நிறுத்தப்பட்டது):

`podman ps --all`

- ஒன்று அல்லது அதற்கு மேற்பட்ட கொள்கலன்களைத் தொடங்கவும்:

`podman start {{கொள்கலன்_பெயர்}} {{கொள்கலன்_ஐடி}}`

- ஒன்று அல்லது அதற்கு மேற்பட்ட இயங்கும் கொள்கலன்களை நிறுத்துங்கள்:

`podman stop {{கொள்கலன்_பெயர்}} {{கொள்கலன்_ஐடி}}`

- பதிவேட்டில் இருந்து ஒரு படத்தை இழுக்கவும் (டாக்கர் ஹப்பிற்கு இயல்புநிலை):

`podman pull {{படத்தின்_பெயர்}}:{{படத்தின்_டேக்}}`

- ஏற்கனவே இயங்கும் கொள்கலனில் ஒரு ஷெல் திறக்க:

`podman exec --interactive --tty {{கொள்கலன்_பெயர்}} {{sh}}`

- ஒன்று அல்லது அதற்கு மேற்பட்ட நிறுத்தப்பட்ட கொள்கலன்களை அகற்றவும்:

`podman rm {{கொள்கலன்_பெயர்}} {{கொள்கலன்_ஐடி}}`

- ஒன்று அல்லது அதற்கு மேற்பட்ட கொள்கலன்களின் பதிவுகளைக் காண்பி மற்றும் பதிவு வெளியீட்டைப் பின்பற்றவும்:

`podman logs --follow {{கொள்கலன்_பெயர்}} {{கொள்கலன்_ஐடி}}`