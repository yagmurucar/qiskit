# QAOA'nın Temel Prensipleri
# QAOA, iki tür Hamiltonian kullanır:

# Cost Hamiltonian (H_C): Bu, çözmek istediğiniz optimizasyon problemini temsil eder.
# Mixer Hamiltonian (H_M): Bu, sistemin durumunu karıştırarak farklı çözümleri keşfetmeyi sağlar.

# 1. Problemin Tanımlanması
# Örneğin, Max-Cut problemini ele alalım. Max-Cut, bir grafın düğümlerini iki kümeye ayırarak, bu kümeler arasındaki 
# kesişen kenarların toplam ağırlığını maksimize etmeyi amaçlar.

# 2. Hamiltonian'ların Tanımlanması
# Cost Hamiltonian (H_C): Bu, kesişen kenarların sayısını temsil eder.

# Mixer Hamiltonian (H_M): Genellikle tüm qubit'ler üzerinde bir X kapısı (Pauli-X operatörü) kullanılarak tanımlanır.

##HAMİLTONİAN OPERATÖRÜ NE İŞE YARAR
# Cost Hamiltonian (𝐻𝐶HC):

# Bu Hamiltonian, çözmek istediğiniz optimizasyon problemini tanımlar.
# Örneğin, Max-Cut problemi için 
# 𝐻𝐶HC kesişen kenarların sayısını veya ağırlığını temsil eder.
# Mixer Hamiltonian (𝐻𝑀HM):

# Bu Hamiltonian, sistemin farklı olası çözümler arasında geçiş yapmasını sağlar.
# Genellikle tüm qubit'ler üzerinde bir X kapısı (Pauli-X operatörü) kullanılarak tanımlanır.
#  SÜPERPOSZİSYON; Qubit, aynı anda hem 0 hem de 1 durumunda olabilir. Matematiksel olarak, bir qubit durumu a+b=1 süperpozisyon oldugunu gösterir
# Dolanıklık:
# Qubitler, birbirleriyle dolanık hale getirilebilir. 
# Bu, iki veya daha fazla qubitin durumlarının birbirine bağlı olduğu anlamına gelir.
# Bir qubitin durumunu ölçmek, dolanık olduğu diğer qubitlerin durumunu da etkiler.
# Ölçüm:

# Bir qubit ölçüldüğünde, belirli bir olasılıkla 0 veya 1 durumunda bulunur. 
# Ölçüm sonucunda, qubit süperpozisyon durumundan klasik bir 0 veya 1 durumuna çöker.

; X Kapısı (Pauli-X): Qubit'in durumunu tersine çevirir.
; H Kapısı (Hadamard): Qubit'i süperpozisyona getirir.
; CNOT Kapısı: İki qubit arasında kontrol edici bir kapıdır ve dolanıklık oluşturmak için kullanılır.
