<!-- ELUCENIA technical documentation · funcao-discriminante-de-maddrey · hi · no clinical/professional/rights approval -->

# Maddrey डिस्क्रिमिनेंट फ़ंक्शन

[शर्तें, स्रोत और अनुमतियाँ](https://elucenia.org/hi/tools/funcao-discriminante-de-maddrey)

## उपयोग कैसे करें

पोर्टल पर उपकरण का उपयोग करें या स्थानीय HTTP सर्वर के माध्यम से index.html खोलें। भाषा चुनें, फ़ील्ड भरें और गणना करें।

## इनपुट और इकाइयाँ

### रोगी का प्रोथ्रोम्बिन समय

`tp`

s · सीमा: 5–150

### नियंत्रण प्रोथ्रोम्बिन समय

`tpc`

s · सीमा: 5–30

### कुल बिलीरुबिन

`bili`

mg/dL · सीमा: 0.1–80

## विधि का संस्करण

संशोधित Maddrey/Carithers 1989: 4.6×(रोगी PT−नियंत्रण PT)+बिलिरुबिन; मूल 1978 निरपेक्ष PT समीकरण नहीं

## दस्तावेज़ित सूत्र

डिस्क्रिमिनेंट फ़ंक्शन = 4.6 × (रोगी का PT − नियंत्रण PT, सेकंड में) + कुल बिलीरुबिन (mg/dL)।

## सीमाएँ और जनसमूह

मूल 1978 फ़ंक्शन का अध्ययन अल्कोहलीय हेपेटाइटिस में हुआ था। स्थानीय संशोधित रूप, जिसमें प्रोथ्रोम्बिन समय का अंतर और 32 कटऑफ है, बाद के 1989 संस्करण के अनुरूप होना चाहिए। कुल स्कोर किसी भी उपचार निर्णय से पहले निषेधों, संक्रमण और वैकल्पिक निदानों के मूल्यांकन का विकल्प नहीं है।

## संदर्भ

- [Maddrey WC et al. Corticosteroid therapy of alcoholic hepatitis. Gastroenterology, 1978.](https://doi.org/10.1016/0016-5085(78)90401-8)

- [Carithers RL et al. Methylprednisolone therapy in patients with severe alcoholic hepatitis: a randomized multicenter trial. Ann Intern Med, 1989.](https://doi.org/10.7326/0003-4819-110-9-685)

- [Crabb DW et al. Diagnosis and treatment of alcohol-associated liver diseases: 2019 practice guidance from the American Association for the Study of Liver Diseases. Hepatology, 2020.](https://doi.org/10.1002/hep.30866)

## तकनीकी परीक्षण दोहराएँ

दर्ज कृत्रिम मामलों को दोहराने के लिए इस रिपॉज़िटरी की मूल निर्देशिका में node test.cjs चलाएँ। मूल इनपुट, अपेक्षित परिणाम और सहनशीलता सीमाएँ सुरक्षित रखी गई हैं। तकनीकी परीक्षण नैदानिक सत्यापन नहीं हैं।

```sh
node test.cjs
```

tool.json में स्रोत, संस्करण और समीक्षा का दायरा दिया गया है। examples.json में कृत्रिम इनपुट और अपेक्षित परिणाम सुरक्षित हैं; results.json में प्राप्त परिणाम दर्ज हैं।

[रिकॉर्ड और संदर्भ](../tool.json) · [JavaScript कोड](../calculator.js) · [संदर्भ मामले](../examples.json) · [results.json](../results.json)

## समीक्षा और उपयोग की शर्तें

स्वतंत्र नैदानिक समीक्षा नहीं की गई है।

यह इंटरफ़ेस लेखकों द्वारा किया गया अनुवाद है, कोई आधिकारिक या प्रमाणित संस्करण नहीं। स्वतंत्र नैदानिक समीक्षा, पेशेवर भाषाई समीक्षा और उपकरणों के अधिकारों की अनुमति की प्रक्रिया पूरी नहीं हुई है।

सूत्र या वर्गीकरण का परिणाम। व्याख्या, कार्यवाही और उपयुक्तता पेशेवर मूल्यांकन और चुने गए स्रोत पर निर्भर है।

## लाइसेंस और श्रेय

Apache-2.0 केवल ELUCENIA के कोड पर लागू होता है। उपकरणों, प्रकाशनों, अनुवादों और डेटा के अधिकार उनके संबंधित अधिकारधारकों के पास रहते हैं। LICENSE और NOTICE सुरक्षित रखें।

ELUCENIA · Felipe Guedes · Copyright © 2026
