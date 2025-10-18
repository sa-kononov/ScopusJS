# ScopusJS.html
Browser app on JavaScript for searching scientific publications via free Scopus Search API. 
Download _ScopusJS.html_ on your PC and open in any modern web browser. No special permissions are needed. To use it one has to obtain an Elsevier's development API key on https://dev.elsevier.com/ (free registration) and enter it in the form. For frequent use one may include an API key in the code as a value of the input#apikey element.

# ScopusPureJS.html
Scopus and Pure clients combined. Check a Pure CRIS for publications found in Scopus and show Pure ID along with document IDs from Scopus.
Download _ScopusPureJS.html_ on your PC and open in any modern web browser. To use it one has to obtain an Elsevier's development API key on https://dev.elsevier.com/ (free registration) and enter it in the form. For frequent use one may include an API key in the code as a value of the input#apikey element. 

One also needs to change three parameters in the JS code as commented:
<pre>
// In the values of pureEndpoint и pureUrlTemplate replace <your.pure.server> with the name of your Pure server, i.e. pure.nsu.ru
// Replace <api-version> with the actual WS API version enabled for your Pure installation, i.e. 524
const pureEndpoint = 'https://<your.pure.server>/ws/api/<api-version>/research-outputs'; 
const pureUrlTemplate = 'https://<your.pure.server>/admin/editor/dk/atira/pure/api/shared/model/researchoutput/editor/{pureType}editor.xhtml?scheme=&type=&id={pureId}';
// Insert an API key for Pure WS as the value of pureApiKey. 
// API key is to be registered in the 'Administration->Api keys' tab of the Pure backend with access to endpoints: Research output, Journal.
</pre>
