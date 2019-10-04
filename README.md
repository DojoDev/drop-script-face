# Drop Monstro Script Events Pixel FAcebook
Script para o evento de Purchase No Facebook Pixel

#COPIE SOMENTE O CÒDIGO APÓS A LINHA

------------------------------------------------------------------------------------------------------------------------------

javascript:(function(){ var codigo = document.getElementById("ProductJson-product-template"); if(codigo == undefined){ content_id = meta["product"]["id"]; } else { var content_id = JSON.parse(codigo.text)["id"].toString(); } fbq('track', 'Purchase', { content_type: 'product_group', content_ids: '[' + content_id + ']' , value: 99.00, num_items: 1, currency: 'USD', }); console.log("O pixel de PUR foi ativado com sucesso para o content ID: " + content_id); })();
