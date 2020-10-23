# js-packages


//main purpose is to convert params to query string url
function convertObjToUrl(objParams){
    let queryString = '';

    if(typeof objParams == 'object') {
        Object.keys(objParams).forEach(function (key) {
            if (objParams[key] !== 'undefined') {
                queryString += key + '=' + objParams[key] + '&';
            }
        });
    }
    return queryString;
}
