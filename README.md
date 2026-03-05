La presente tesi ha analizzato la capacità predittiva e operativa di modelli quantitativi applicati ai 
rendimenti giornalieri di Bitcoin, con particolare attenzione a strutture ibride che combinano modelli 
econometrici lineari (ARIMA, ARFIMA) con algoritmi di Machine Learning e architetture di Deep 
Learning. L’intero framework sperimentale è stato costruito secondo un’impostazione rigorosamente 
time-consistent, basata su validazione walk-forward expanding window e su metriche calcolate 
esclusivamente out-of-sample, al fine di garantire risultati metodologicamente robusti e privi di bias 
informativi. I risultati empirici mostrano in modo chiaro come, nel contesto giornaliero di Bitcoin, la 
prevedibilità direzionale dei rendimenti sia estremamente limitata. Nessuna delle architetture 
considerate, né i modelli econometrici lineari, né gli ensemble di algoritmi di Machine Learning, né 
le reti LSTM, è riuscita a superare in modo significativo il benchmark casuale. Le accuratezze si 
collocano stabilmente intorno allo 0,50, mentre i valori di ROC-AUC risultano inferiori o prossimi a 
0,50, indicando l’assenza di una struttura discriminativa sfruttabile. In particolare, l’integrazione delle 
previsioni ARIMA e ARFIMA come feature additive nei modelli non lineari non ha prodotto un 
miglioramento sostanziale delle performance. L’analisi di interpretabilità tramite SHAP ha 
confermato che il contributo informativo delle previsioni econometriche è marginale, mentre il 
modello ensemble tende a basarsi quasi esclusivamente sui lag dei rendimenti, che tuttavia presentano 
contributi instabili e privi di una relazione strutturata con la variabile target. Anche le architetture 
LSTM, pur teoricamente più flessibili e capaci di modellare dipendenze temporali non lineari, non 
hanno mostrato un vantaggio competitivo rispetto agli ensemble di Machine Learning, confermando 
la difficoltà di estrarre pattern stabili dai rendimenti giornalieri di Bitcoin. Dal punto di vista 
operativo, la costruzione di una strategia direzionale long/short basata sulle previsioni dell’ensemble 
ML ha evidenziato risultati fortemente negativi. Una volta incorporati costi di transazione dinamici, 
modellati come funzione crescente della volatilità condizionata stimata tramite GARCH (1,1), la 
strategia presenta rendimenti medi negativi, Sharpe e Sortino ratio ampiamente inferiori a zero e un 
massimo drawdown prossimo al −100%. Tali evidenze indicano che il debole potere predittivo dei 
modelli non è sufficiente a compensare l’elevata volatilità dell’asset e le frizioni di mercato 
realistiche. Nel complesso, i risultati empirici convergono verso una conclusione chiara, ovvero nel 
periodo analizzato e a frequenza giornaliera, il mercato di Bitcoin mostra un comportamento 
compatibile con un processo altamente rumoroso e prossimo a una martingala, rendendo inefficaci le 
strategie direzionali basate esclusivamente sulla previsione del segno dei rendimenti. 
