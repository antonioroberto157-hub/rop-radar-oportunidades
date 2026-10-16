# Relatório de auditoria do catálogo ROP
**Data:** 16/10/2026  
**Escopo:** revisão estática dos 194 registros em `catalogo.html`, correções no branch `audit/correcoes-catalogo-2026-10`. Não houve publicação.

## Resumo da inspeção estática
- Registros de produtos: 194.
- Com custo numérico: 108.
- Com preço de varejo/referência numérico: 65.
- Com ambos os valores: 52.
- Sem nenhum dos dois valores: 73.
- Sem URL de fornecedor específica cadastrada: 97.
- URLs de pesquisa Google em vez de página de produto: 23.
- Registros com URL de pesquisa/listagem no campo principal ou de varejo: 100 (contagem por produto; não significa link quebrado).
- Pares de URLs de compra e varejo no mesmo domínio: 0; domínio diferente não prova SKU equivalente.
- Datas de verificação preenchidas: 0. Todos os registros ficam pendentes até uma conferência real; campos estruturados foram adicionados sem inventar datas, SKUs ou condições.
- Links não foram tratados como quebrados apenas por serem páginas de busca, exigirem JavaScript, bloquearem robôs ou pedirem seleção de variação.

## Alterações realizadas
1. Removida a lista fixa de IDs que limitava a vitrine e ocultava produtos existentes.
2. O status de validação exige fontes separadas, SKU/variante confirmado e datas estruturadas de conferência. Como essas evidências não estavam registradas nos campos próprios, nenhum produto é automaticamente promovido a validado.
3. Adicionados campos por produto: SKU, confirmação de equivalência, data de verificação do fornecedor, data de verificação do preço, mínimo de unidades, status de frete e status das taxas. Valores desconhecidos permanecem explicitamente pendentes.
4. Atualizada a referência de varejo do TP-Link Archer T2U Plus para uma página específica da Pichau; custo do fornecedor ficou pendente devido à inconsistência de estoque observada.
5. Mini processador Original Line 0234D: custo atualizado para R$ 8,99 no Pix e referência de varejo não equivalente removida.
6. Removidas referências de varejo numéricas que não tinham SKU/variante comprovadamente equivalente para câmera infantil, karaokê, caixa de som 30 W, carrinho RC com fumaça, copo térmico 1,2 L, caranguejo musical e Squishy Baozi. Esses preços precisam ser reintroduzidos apenas após nova verificação.

## Produtos sem URL de fornecedor específica
- SSD Kingston NV3 — 1 TB (`ssd`)
- SSD SATA — 480/500 GB (`ssd-sata`)
- SSD NVMe — 500/512 GB (`ssd-512`)
- Mouse Logitech G102 (`mouse`)
- Mouse sem fio 2.4 GHz (`mouse-sem-fio`)
- Teclado USB básico (`teclado`)
- Teclado mecânico de entrada (`teclado-mec`)
- Headset com microfone (`headset`)
- Mousepad grande (`mousepad`)
- Webcam USB 1080p (`webcam`)
- Memória RAM DDR4 — 8 GB (`ram8`)
- Memória RAM DDR4 — 16 GB (`ram16`)
- Hub USB — 4 portas (`hub`)
- Adaptador TP-Link Archer T2U Plus AC600 (`wifi-t2u`)
- Adaptador Wi-Fi USB (`wifi`)
- Roteador Wi-Fi de entrada (`router`)
- Cabo USB-C reforçado (`cabo`)
- Carregador USB-C 20 W (`carregador`)
- Suporte para notebook (`suporte`)
- Power bank — bateria portátil (`powerbank`)
- Fita LED USB (`led`)
- Tomada inteligente Wi-Fi (`tomada`)
- Organizador de cabos (`organizador`)
- Kit de precisão para eletrônicos (`ferramentas`)
- Trena métrica de 5 metros (`trena`)
- Bebedouro portátil para pets (`pet`)
- Brinquedo interativo para pets (`pet-brinquedo`)
- Suporte veicular para celular (`suporte-veicular-para-celular`)
- Tripé ajustável para celular (`tripe-ajustavel-para-celular`)
- Ring light com suporte (`ring-light-com-suporte`)
- Carregador portátil MagSafe compatível (`carregador-portatil-magsafe-compativel`)
- Cabo Lightning para iPhone (`cabo-lightning-para-iphone`)
- Cabo USB-C trançado (`cabo-usb-c-trancado`)
- Adaptador USB-C para USB-A (`adaptador-usb-c-para-usb-a`)
- Suporte de mesa para celular (`suporte-de-mesa-para-celular`)
- Caixa de som Bluetooth portátil (`caixa-de-som-bluetooth-portatil`)
- Microfone de lapela USB-C (`microfone-de-lapela-usb-c`)
- Microfone USB para computador (`microfone-usb-para-computador`)
- Suporte articulado para microfone (`suporte-articulado-para-microfone`)
- Cabo P2 auxiliar (`cabo-p2-auxiliar`)
- Adaptador Bluetooth USB (`adaptador-bluetooth-usb`)
- Controle remoto para apresentação (`controle-remoto-para-apresentacao`)
- Lâmpada LED bulbo (`lampada-led-bulbo`)
- Luminária de mesa LED (`luminaria-de-mesa-led`)
- Extensão elétrica com tomadas (`extensao-eletrica-com-tomadas`)
- Filtro de linha (`filtro-de-linha`)
- Luz noturna de presença (`luz-noturna-de-presenca`)
- Luminária de emergência recarregável (`luminaria-de-emergencia-recarregavel`)
- Pilha alcalina AA — kit (`pilha-alcalina-aa-kit`)
- Balança digital de cozinha (`balanca-digital-de-cozinha`)
- Kit de potes herméticos (`kit-de-potes-hermeticos`)
- Kit de utensílios de silicone (`kit-de-utensilios-de-silicone`)
- Abridor multifuncional (`abridor-multifuncional`)
- Afiador manual de facas (`afiador-manual-de-facas`)
- Garrafa de água reutilizável (`garrafa-de-agua-reutilizavel`)
- Caneca térmica (`caneca-termica`)
- Organizador de temperos (`organizador-de-temperos`)
- Lixeira compacta para carro (`lixeira-compacta-para-carro`)
- Aspirador portátil para carro (`aspirador-portatil-para-carro`)
- Kit de escovas de limpeza automotiva (`kit-de-escovas-de-limpeza-automotiva`)
- Medidor de pressão de pneus (`medidor-de-pressao-de-pneus`)
- Organizador de porta-malas (`organizador-de-porta-malas`)
- Pano de microfibra automotivo (`pano-de-microfibra-automotivo`)
- Kit de faixas elásticas fitness (`kit-de-faixas-elasticas-fitness`)
- Corda de pular ajustável (`corda-de-pular-ajustavel`)
- Squeeze esportivo (`squeeze-esportivo`)
- Luvas para musculação (`luvas-para-musculacao`)
- Tapete para yoga e exercícios (`tapete-para-yoga-e-exercicios`)
- Rolo de liberação miofascial (`rolo-de-liberacao-miofascial`)
- Necessaire organizadora (`necessaire-organizadora`)
- Carteira compacta (`carteira-compacta`)
- Cinto casual ajustável (`cinto-casual-ajustavel`)
- Estojo rígido para óculos (`estojo-rigido-para-oculos`)
- Bolsa transversal compacta (`bolsa-transversal-compacta`)
- Organizador de bijuterias (`organizador-de-bijuterias`)
- Organizador de maquiagem (`organizador-de-maquiagem`)
- Kit de pincéis de maquiagem (`kit-de-pinceis-de-maquiagem`)
- Espelho compacto com luz (`espelho-compacto-com-luz`)
- Touca de cetim para cabelo (`touca-de-cetim-para-cabelo`)
- Massageador facial manual (`massageador-facial-manual`)
- Escova massageadora de couro cabeludo (`escova-massageadora-de-couro-cabeludo`)
- Caderno universitário (`caderno-universitario`)
- Kit de canetas esferográficas (`kit-de-canetas-esferograficas`)
- Kit de marca-textos (`kit-de-marca-textos`)
- Etiquetas adesivas multiuso (`etiquetas-adesivas-multiuso`)
- Fita adesiva para embalagem (`fita-adesiva-para-embalagem`)
- Tesoura de escritório (`tesoura-de-escritorio`)
- Organizador de mesa (`organizador-de-mesa`)
- Kit de babadores para bebê (`kit-de-babadores-para-bebe`)
- Organizador de fraldas (`organizador-de-fraldas`)
- Mordedor de silicone para bebê (`mordedor-de-silicone-para-bebe`)
- Babador impermeável infantil (`babador-impermeavel-infantil`)
- Organizador de brinquedos infantil (`organizador-de-brinquedos-infantil`)
- Capa de chuva compacta (`capa-de-chuva-compacta`)
- Kit de organizadores de mala (`kit-de-organizadores-de-mala`)
- Cadeado para mala (`cadeado-para-mala`)
- Necessaire de viagem (`necessaire-de-viagem`)

## Produtos cujo campo principal é uma pesquisa Google
Esses endereços são buscas dinâmicas e não foram classificados como links quebrados. Devem ser substituídos por páginas de produto específicas quando uma oferta comparável for identificada.

- SSD SATA — 480/500 GB (`ssd-sata`)
- SSD NVMe — 500/512 GB (`ssd-512`)
- Mouse sem fio 2.4 GHz (`mouse-sem-fio`)
- Teclado USB básico (`teclado`)
- Teclado mecânico de entrada (`teclado-mec`)
- Headset com microfone (`headset`)
- Mousepad grande (`mousepad`)
- Webcam USB 1080p (`webcam`)
- Memória RAM DDR4 — 8 GB (`ram8`)
- Memória RAM DDR4 — 16 GB (`ram16`)
- Adaptador Wi-Fi USB (`wifi`)
- Roteador Wi-Fi de entrada (`router`)
- Cabo USB-C reforçado (`cabo`)
- Carregador USB-C 20 W (`carregador`)
- Suporte para notebook (`suporte`)
- Power bank — bateria portátil (`powerbank`)
- Fita LED USB (`led`)
- Tomada inteligente Wi-Fi (`tomada`)
- Organizador de cabos (`organizador`)
- Kit de precisão para eletrônicos (`ferramentas`)
- Trena métrica de 5 metros (`trena`)
- Bebedouro portátil para pets (`pet`)
- Brinquedo interativo para pets (`pet-brinquedo`)

## Limites e próximos passos
- Esta auditoria estática não confirma o status HTTP de todos os links, estoque, preço final, frete por CEP ou condições comerciais de cada fornecedor.
- As 194 referências ainda precisam de verificação individual de SKU/modelo, quantidade por embalagem, lote mínimo, preço com forma de pagamento, data/hora, frete, impostos e taxas do canal de venda.
- Links de pesquisa/listagem são pistas para encontrar ofertas, não evidência de preço atual ou de produto idêntico.
- Nenhuma margem deve ser considerada validada até que a fonte de compra e a fonte de varejo sejam específicas e comparáveis.
