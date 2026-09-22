# Week 2 — Mathematical Preliminaries

> Syllabus (TR): *Matematiksel önbilgiler*

**Previous:** [Week 1](01-course-overview.md) · **Next:** [Week 3](03-regular-languages-finite-automata.md)

## Goals
- Use sets, sequences, tuples, functions, relations and graphs precisely.
- Write a proof by construction, contradiction, and induction.

## Key concepts
- Alphabet Σ, string, length, empty string ε, concatenation, Σ*.
- Language = a set of strings over Σ. This is the object of the whole course.
- Proof techniques: construction, contradiction, induction — every later theorem uses one.
- Diagonalization (preview) — the tool that will show some languages are undecidable.

## Reading

- [Sipser — Ch. 0.2 (mathematical notions and terminology)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=27)
- [Sipser — Ch. 0.3 (definitions, theorems, and proofs)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=41)
- [Sipser — Ch. 0.4 (types of proof)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=45)

## Practice
- [ ] Do Sipser exercises 0.1-0.13
- [ ] Write one induction proof end-to-end without looking at the book

## Checklist
- [ ] Lecture attended
- [ ] Textbook section read
- [ ] Exercises done
- [ ] Notes written below

---

This file is the shared plan — improve it if the course changes, but keep it general.
Personal notes go below, one `## Notes — <Name> (<term>)` section per person.

## Notes — Efe (2026-2027 Fall)

### Lecture

1.1 FINITE AUTOMATA 
:


<!-- What was actually covered, and what the lecturer emphasised. -->
https://muratakcs.github.io/cse435/

recognizes language 

DEFINITION 1.16 
### Worked out by hand
<!-- Derivations, proofs, traced algorithms. -->

data uızerinde islem yaparkanki hafiza? state machine emirhanla yaptığımız dan mı bahsediyor acaba?

regular lang - -> hafıza olmadan. ( language manipulation --> problem )  
language -- > bir alfabe var ve o alfabe ile uretebildigimiz degerler language . 

- ALFABE - > LANGUAGE - > VE LANGUAGE UZERINDE YAPTIGIMIZ BIR ISLEM. 
- data representationu - - - renk, satranc . 
- graph i nasil represente edecegiz? mesela ( elemanları * elemanların ilişkisi ) gibi bir sey icat edilebilir ornegin. bu representationların da en kısa en tutarlı vs. her ne denilirse versiyonları da bizim languagemiz oluyor sanirim ?  yani o graphların hepsi o dilin elemanı olmus oluyor. Formal Languages...

---
Deterministic Finite Automata 

O - Rejected State
OO - Accepted State

odd until now, even until now state leri . . . even or not even. 

start with reverse ????( sipsar kitapta varmis )

dfa minimization algorithm 


even numbers in binary (E) dfa sini construct ettik. sonra bunu reverse şekilde daha kolay olur diye düşünüp aslında yeni bi language oluşturduk. fakat leading zeros problemi ile karşılaştık ve onu çözdük vs. vs. bir ornek olarak . 

**markov chains** 
transitionlar oklar oluyor. 

bir stringi compute ederken. kaç farklı state e ihtiyacım olabilir. ? 





### Questions
<!-- Unclear things. Ask, then answer them here. -->
closure ? nedir ? bu bir özellik midir? teoride cok kullanisliymis ? 

> **Açıklama:** Evet, bir özellik. Bir language class'ı (mesela tüm regular language'lar) bir işleme göre **closed** ise, o class'tan iki language alıp işlemi uyguladığında sonuç yine aynı class'ın içinde kalır. Tam sayılar toplamaya göre closed'dır: iki tam sayıyı toplarsan yine tam sayı elde edersin. Bölmeye göre closed değildir, çünkü 1/2 tam sayı değil. Regular language'lar complement, union, concatenation ve star işlemlerine göre closed (Sipser Theorem 1.25–1.26, ileride gelecek). Neden kullanışlı? Basit DFA'lardan karmaşık language'ları "bedavaya" kurabiliyorsun. Ayrıca bir language'ın regular **olmadığını** göstermek için de kullanılıyor. Q13 bunun ilk örneği.

#### Practice — Sipser Ch 0 + Ch 1.1 (Example 1.7'ye kadar, s. 37)
<!-- Cevabını "Cevabım:" satırına yaz. Emin değilsen tahminini yaz, sonra birlikte bakarız. -->

##### A. Alphabet, string, language (Ch 0.2)

**Q1.** Σ = {0, 1}. Uzunluğu 2 olan tüm string'leri yaz. Uzunluğu n olan kaç string vardır?
> Cevabım: 00, 01, 10, 11  --- 3 olsa. 000, 001, 010, 011, 100, 101, 110, 111
> 2 de 4 oluyor.  3 de 8 oluyor.  2 üzeri n. oluyor 

> **Açıklama:** Doğru 👍 Her pozisyon için 2 seçenek var (0 ya da 1) ve n pozisyon var. Seçimler bağımsız olduğu için sonuç 2·2·…·2 = **2ⁿ**. Genel hali: |Σ| = k ise uzunluğu n olan string sayısı **kⁿ**. n = 0 için 2⁰ = 1 çıkıyor, o tek string de ε.

**Q2.** ε nedir, |ε| kaçtır? ∅ ile {ε} aynı language mı? Farkları ne?
> Cevabım:  epsilon diğeri boş küme ? 1.7 falan dı sanırım. 

> **Açıklama:** Doğru yoldasın. **ε = empty string**, yani hiç sembol içermeyen string. Uzunluğu **|ε| = 0**. (1.7 ile ilgisi yok. Ama ε'u kabul eden bir makine Example 1.9'da, M3'te var.)
> - **∅** = empty language. **Hiç** string içermez, 0 elemanlı.
> - **{ε}** = sadece empty string'i içeren language, **1** elemanlı.
> - Yani aynı değiller. Kutu benzetmesi: ∅ boş bir kutu, {ε} ise içinde boş bir kağıt olan kutu. Kağıtta bir şey yazmıyor ama kutu boş değil.

**Q3.** x = 01, y = 110. xy, yx ve |xy| nedir? xy = yx mi?
> Cevabım: bilemedim bunu 

> **Açıklama:** **Concatenation** iki string'i uç uca eklemek demek, araya hiçbir şey girmiyor.
> - xy = 01 + 110 = **01110**
> - yx = 110 + 01 = **11001**
> - |xy| = 2 + 3 = **5**. Genel kural: |xy| = |x| + |y|.
> - xy ≠ yx, çünkü concatenation **commutative değil**, sıra önemli. Ama associative: (xy)z = x(yz). Bir de ε etkisiz eleman: xε = εx = x.

**Q4.** Σ* nedir? Sonlu mu sonsuz mu? Σ = {0,1} üzerindeki her language Σ*'ın alt kümesi midir?
> Cevabım: sonsuzdur. evet alt kumesidir. 

> **Açıklama:** İkisi de doğru 👍 **Σ\*** = Σ'dan yazılabilecek **bütün sonlu string'ler**, ε dahil: {ε, 0, 1, 00, 01, …}. Küme sonsuz ama içindeki her string sonlu uzunlukta, bu ayrım önemli. Language zaten "Σ\*'ın bir alt kümesi" diye tanımlanıyor, o yüzden her language L ⊆ Σ\* olmak zorunda.

**Q5.** A = {a, b}. P(A) (power set) nedir, kaç elemanı var? Bonus: "Σ üzerindeki bir language" P(Σ*) ile nasıl ilişkili?
> Cevabım: 

> **Açıklama:** **Power set** P(A), A'nın bütün alt kümelerinin kümesi demek.
> - P({a,b}) = { ∅, {a}, {b}, {a,b} }, yani **4 = 2²** eleman. Genel kural: |A| = n ise |P(A)| = **2ⁿ**, çünkü her eleman için "alayım mı, almayayım mı" diye 2 seçenek var.
> - Bonus: L bir language ise L ⊆ Σ\*, bu da **L ∈ P(Σ\*)** demek. Yani Σ üzerindeki bütün language'ların kümesi tam olarak P(Σ\*). İleride bu kümenin "çok fazla" eleman içerdiğini (uncountable) göreceğiz. Makineler (DFA, TM) ise sayılabilir çoklukta, yani countable. Bu yüzden hiçbir makinenin tanıyamadığı language'lar var. Diagonalization'ın fikri bu.

##### B. Proof techniques (Ch 0.4)

**Q6.** Induction ile kanıtla: 1 + 2 + … + n = n(n+1)/2. Üç parçayı ayrı ayrı yaz: base case, induction hypothesis, induction step.
> Cevabım:

> **Açıklama:** Induction'ı domino gibi düşün: ilk taşı düşürürsün (base case), sonra her taşın bir sonrakini düşürdüğünü gösterirsin (step).
> - **Base case (n = 1):** Sol taraf 1. Sağ taraf 1·2/2 = 1. Eşitler ✓
> - **Induction hypothesis:** Formülün bir k için doğru olduğunu varsay: 1 + … + k = k(k+1)/2.
> - **Induction step (k → k+1):** 1 + … + k + (k+1) toplamında ilk k terimin yerine hypothesis'i koy: k(k+1)/2 + (k+1) = (k+1)(k/2 + 1) = **(k+1)(k+2)/2**. Bu da formülün n = k+1 için yazılmış hali ✓
> - Sonuç: base case ve step birlikte doğru olduğu için formül her n ≥ 1 için doğru.

**Q7.** Proof by contradiction'ın mantığı ne? "√2 irrasyoneldir" kanıtının adımlarını kendi cümlelerinle anlat.
> Cevabım:

> **Açıklama:** Mantık şu: kanıtlamak istediğin şeyin **tersini varsay** ve bu varsayımdan bir **çelişki** çıkar. Çelişki çıktıysa varsayım yanlış demektir, o zaman orijinal iddia doğru.
> 1. Tersini varsay: √2 rasyonel olsun, yani √2 = m/n. Kesri **sadeleştirilmiş** kabul et: m ve n'nin ortak böleni yok.
> 2. İki tarafın karesini al: 2 = m²/n², buradan m² = 2n². Yani m² çift, dolayısıyla m de çift. m = 2k yaz.
> 3. Yerine koy: 4k² = 2n², buradan n² = 2k². Yani n de çift.
> 4. m ve n ikisi de çift, ikisi de 2'ye bölünüyor. Bu, "kesir sadeleştirilmiş" varsayımıyla **çelişiyor** ⚡ Demek ki √2 irrasyonel.

##### C. Finite automata (Ch 1.1, Example 1.7'ye kadar)

M1'in transition tablosu (start q1, F = {q2}):

| δ  | 0  | 1  |
|----|----|----|
| q1 | q1 | q2 |
| q2 | q3 | q2 |
| q3 | q2 | q2 |

**Q8.** M1'i şu input'larda çalıştır, geçtiğin state'leri sırayla yaz, accept/reject söyle: `1101`, `0100`, `10`, `ε`.
> Cevabım:

> **Açıklama:** Tabloyu kullanarak soldan sağa her sembolü sırayla oku.
> - `1101`: q1 →1→ q2 →1→ q2 →0→ q3 →1→ **q2** → accept ✓
> - `0100`: q1 →0→ q1 →1→ q2 →0→ q3 →0→ **q2** → accept ✓ (son 1'den sonra 2 tane 0 var, yani çift sayıda)
> - `10`: q1 →1→ q2 →0→ **q3** → reject ✗ (son 1'den sonra tek sayıda 0 var)
> - `ε`: Hiç sembol okunmuyor, makine q1'de kalıyor. q1 accept state değil → reject ✗
> - L(M1) = {w | w en az bir 1 içerir ve son 1'den sonra **çift sayıda** 0 gelir}. q2 ile q3 arasındaki gidip gelme, 0'ların tek mi çift mi olduğunu takip ediyor. Derste gördüğün "even/odd until now" state'leri tam olarak bu.

**Q9.** M1'in 5-tuple'ını yaz: (Q, Σ, δ, q0, F). Her parça ne anlama geliyor, bir cümleyle açıkla.
> Cevabım:

> **Açıklama:**
> - **Q** = {q1, q2, q3}: makinenin bulunabileceği durumlar. Makinenin "hafızası" bunlardan ibaret.
> - **Σ** = {0, 1}: input'ta görülebilecek semboller.
> - **δ** = yukarıdaki tablo. "Şu state'teyken şu sembolü okursam nereye giderim?" sorusunun cevabı.
> - **q0** = q1: başlangıç state'i. Diyagramda "boşluktan gelen ok" ile gösteriliyor.
> - **F** = {q2}: accept state'leri, diyagramda çift halka. Input bittiğinde makine burada duruyorsa accept.

**Q10.** δ : Q × Σ → Q. Domain ne, range ne? |Q| = 3 ve |Σ| = 2 ise tabloda kaç hücre olur? Neden her state'ten her sembol için **tam bir** ok çıkmak zorunda?
> Cevabım:

> **Açıklama:**
> - **Domain** = Q × Σ, yani (state, sembol) çiftleri. Örneğin (q2, 0).
> - **Range** = Q, yani her çift tek bir state'e gidiyor: δ(q2, 0) = q3.
> - Hücre sayısı |Q| · |Σ| = 3 · 2 = **6**.
> - Neden her state'ten her sembol için tam bir ok? Çünkü δ bir **function**: her input'a **tam olarak bir** output vermek zorunda. Ok hiç yoksa function tanımsız kalır. İki ok varsa makine hangisine gideceğini bilemez. DFA'daki "**D**eterministic" kelimesi buradan geliyor: bir sonraki adım her zaman kesin. (Birden fazla seçeneğe izin veren makineye NFA deniyor, o da yakında gelecek.)

**Q11.** Bir DFA'nın hiç accept state'i olmayabilir mi (F = ∅)? O zaman hangi language'ı recognize eder?
> Cevabım:

> **Açıklama:** Evet, olabilir. F = ∅ olması tanımda serbest (Sipser s. 36). Makine hiçbir string'i kabul etmez, bu yüzden tanıdığı language **∅** olur. Dikkat: bu {ε} değil! (Q2 ile bağlantısına bak.) Bir makine hiç string kabul etmese bile yine **bir** language recognize eder, o da empty language.

**Q12.** M2 (Example 1.7): start q1, F = {q2}, δ(q, 0) = q1, δ(q, 1) = q2. `1101`, `110`, `ε` accept mi? L(M2) nedir?
> Cevabım:

> **Açıklama:** M2'nin kuralı çok basit: 0 okuyunca q1'e, 1 okuyunca q2'ye git. Hangi state'te olduğun önemli değil. Yani M2 sadece "**son okuduğum sembol neydi?**" bilgisini hatırlıyor.
> - `1101`: q1 → q2 → q2 → q1 → **q2** → accept ✓
> - `110`: q1 → q2 → q2 → **q1** → reject ✗
> - `ε`: q1'de kalıyor → reject ✗
> - **L(M2) = {w | w 1 ile biter}**

**Q13.** M2'yi değiştirerek "1 ile **bitmeyen**" string'leri tanıyan DFA yap. Neyi değiştirdin? (İpucu: bu soru closure sorusuna bağlanıyor.)
> Cevabım:

> **Açıklama:** Tek yapman gereken **accept ve non-accept state'lerin yerini değiştirmek**: F = {q2} yerine F = {q1}. Transition'lara dokunmuyorsun.
> - Artık 0 ile biten string'ler **ve ε** kabul ediliyor. ε de "1 ile bitmeyen" bir string, yani doğru davranış bu.
> - Bu yöntem her DFA'da işe yarar: F yerine **Q − F** koyarsan makine tam tersi language'ı tanır. Buna **complement** deniyor.
> - Bunun sonucu olarak **regular language'lar complement'e göre closed**. Bir language'ı bir DFA tanıyorsa, complement'ini de bir DFA tanır. En üstteki closure sorusunun cevabının ilk parçası bu.

##### D. Derste yaptıklarımız

**Q14.** Σ = {0,1}. "Çift sayıda 0 içeren" string'leri tanıyan DFA tasarla. State'ler ne "hatırlıyor"? Tablo + 5-tuple yaz.
> Cevabım:

> **Açıklama:** Önce şunu sor: "String'i okurken neyi hatırlamam gerekiyor?" Cevap: şu ana kadar görülen 0 sayısının tek mi çift mi olduğu. Başka hiçbir şeyi hatırlamaya gerek yok, o yüzden **2 state** yetiyor.
> - **q_even** (start **ve** accept): "şu ana kadar çift sayıda 0 gördüm". Başta 0 tane 0 var, 0 çift sayı, o yüzden start state bu.
> - **q_odd**: "tek sayıda 0 gördüm"
>
> | δ      | 0      | 1      |
> |--------|--------|--------|
> | q_even | q_odd  | q_even |
> | q_odd  | q_even | q_odd  |
>
> - 5-tuple: ({q_even, q_odd}, {0,1}, δ, q_even, {q_even})
> - 1 okuyunca state değişmiyor, çünkü 1'ler sayılmıyor. ε kabul ediliyor, çünkü içinde 0 tane 0 var ve 0 çift.

**Q15.** Binary'de çift sayılar (E) için DFA. Bir binary sayının çift olup olmadığına hangi bit karar verir? `0010` language'da mı olmalı (leading zeros)? `ε` ne olmalı?
> Cevabım:

> **Açıklama:**
> - Çiftlik kararını **son bit (LSB)** veriyor: binary sayı 0 ile bitiyorsa çift. O zaman DFA'nın "son okunan bit 0 muydu?" bilgisini hatırlaması yeterli. M2'ye çok benziyor.
> - DFA (ε'u reject etmek için 3 state):
>   - **s** (start, henüz hiçbir şey okunmadı)
>   - **z** (son bit 0, **accept**)
>   - **o** (son bit 1)
>   - Her state'ten 0 okuyunca **z**'ye, 1 okuyunca **o**'ya git.
> - **Leading zeros**: `0010` = 2, yani çift bir sayı. Ama "bu string geçerli bir binary sayı mı?" sorusu **tanıma bağlı**. `0010`'u kabul edebiliriz, ya da "sayı 0 ile başlamaz (tek istisna `0`)" kuralı koyup reddedebiliriz. İkinci yolu seçersen o kuralı kontrol eden ek state'ler lazım (bir de "reject edip orada kalan" bir dead state). Derste leading zeros problemini çözerken büyük ihtimalle bu tür bir kural koydunuz. Önemli olan şu: language'ı **sen** tanımlıyorsun, DFA da o tanımı birebir uygulamalı.
> - **ε**: Sayı değil, o yüzden reddetmek mantıklı. s state'inin accept olmamasının sebebi bu.
> - **Reverse**: String'i tersten okursak karar veren bit **ilk** sembol olur. İlk okunan sembol her şeyi belirlediği için DFA daha da kolaylaşır. Derste "reverse daha kolay" demenizin sebebi bu. Hatta bu bir **başka** language'ı tanımlıyor, notlarında yazdığın gibi.


### Exam-worthy
<!-- Formulas, conditions, algorithm steps, pitfalls. -->
