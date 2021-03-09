# Script Mercados Energia
- Scripts Mercados de energia

- Desenvolvendo algoritomo de otimização do despacho hidrotérmico para cada estágio.

- Criando algoritimo da PDDE

- Aplicando Euristicas para melhorar a convergência e performace.

# Sistema

 Nome | ca | cl | Pmax
---------------------
- T1  |  1 | 0  |  30    
- T2  |  2 | 0  |  20    
- T3  |  5 | 0  |  \inf  
 
 Hidro: vmax = 100; qmax = 100; v_inic = 55; y = [5; 30; 45; 40] 

## Formato das Equações de cada Subestágio:

- min f_t = p_1 + 2p_2 + 5_p_3 +\alpha_t
- S.T:
    - p_1 + p_2 + p_3 \geq 80
    - v_t = v_{t-1} + y_t - q_t 
