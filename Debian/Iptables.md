## Iptables

iptables -L # liste toutes les regles existantes
iptables -P INPUT DROP # BLOQUE LES CONNEXIONS ENTRANTES absoluments tout
iptables -F # Flush la chaine selectionner ou toutes les chaines  de la tablessi aucune n'est précisé

#politiques
iptables -P OUTPUT DROP # BLOQUES LES CONNEXIONS SORTANTES
iptables -P INPUT DROP #BLOQUES LES CONNEXIONS ENTRANTES
iptables -P FORWARD DROP # BLOQUES LES CONNEXIONS REDIRIGÉES

#OTHERS
iptables -A INPUT -m state ESTABLISHED,RELATED -j ACCEPT

iptables -A INPUT -p tcp --dport 5789 -j ACCEPT

iptables -A INPUT -i lo -j ACCEPT

iptables -A OUTPUT -o lo -j ACCEPT

iptables -A INPUT -p tcp --dport 80 -j ACCEPT








