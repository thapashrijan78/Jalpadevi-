# श्री जाल्पादेवी माध्यमिक विद्यालय — गुनासो दर्ता प्रणाली

यो परियोजना नेपाली विद्यालय/स्थानीय समुदायका लागि मोबाइल र कम्प्युटर दुवैमा चल्ने गुनासो पोर्टल हो।

## मुख्य सुविधाहरू
- पूर्ण नेपाली UI
- विद्यार्थी, शिक्षक र अभिभावकका लागि गुनासो दर्ता
- व्यक्तिगत विवरण वा गोप्य/अनामिक गुनासो
- गुनासोको विषय, शीर्षक, विवरण र स्थान
- मोबाइल/ल्यापटपबाट आवाज रेकर्ड
- JPG/JPEG/PNG/PDF फाइल संलग्न
- गुनासो दर्ता भएपछि Tracking ID
- Tracking ID बाट गुनासोको अवस्था हेर्ने
- अध्यक्ष/प्रशासनका लागि login
- Admin dashboard, search, filter र status update
- QR code generator — स्क्यान गर्दा सार्वजनिक गुनासो पृष्ठ खुल्ने
- विद्यालयको लोगो/नाम/ठेगाना reference image अनुसार
- Responsive design

## चलाउने तरिका — Mac

### Terminal 1: Backend
```bash
cd ~/Downloads/jalpa-devi-nepali-complaint-portal/backend
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

### Terminal 2: Frontend
```bash
cd ~/Downloads/jalpa-devi-nepali-complaint-portal/frontend
npm install
npm run dev
```

Vite ले दिएको `http://localhost:...` URL browser मा खोल्नुहोस्।

## Demo प्रशासन login
Username: `admin`
Password: `admin123`

## Public pages
- मुख्य पृष्ठ: `#home`
- गुनासो दर्ता: `#complaint`
- गुनासो अवस्था: `#status`
- QR code: `#qr`
- प्रशासन login: `#login`
- प्रशासन dashboard: `#dashboard`

## महत्वपूर्ण
यो local/demo deployment का लागि तयार गरिएको पूर्ण working prototype हो। वास्तविक विद्यालयमा सार्वजनिक प्रयोग गर्दा PostgreSQL, password hashing, HTTPS, secure sessions/JWT, cloud storage, backup, rate limiting र SMS/email notification थप्नुहोस्।
