---
title: Zrozumienie faktury
article_id: 360021047619
translation_id: 360021047619
locale: pl-pl
sidebar_position: 7
created_at: '2021-04-13T06:37:58Z'
updated_at: '2025-10-10T07:52:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Twoje faktury są generowane przez naszego dostawcę rozliczeń, firmę Stripe, i zawierają szczegóły dotyczące zakupu, informacje o firmie, numer paragonu lub faktury oraz używaną metodę płatności." Dowiedz się więcej o tym, jak opłaty, tokeny i korekty są wyświetlane na Twojej fakturze Miro.

> **Dostępne dla**: Abonament Starter, abonament Business
> **Dotyczy:** Administratorzy, administratorzy rozliczeń

## Gdzie znaleźć swoje faktury

### E-maile dotyczące rozliczeń

W ustawieniach rozliczeń możesz określić adres e-mail do otrzymywania wszystkich wiadomości dotyczących rozliczeń. Stripe utworzy paragon i fakturę, a następnie wyśle je na Twój e-mail rozliczeniowy z adresu:

```
faktury+**********@stripe.com
faktury+wyciągi+***************@stripe.com
```

### Ustawienia rozliczeń Miro

Faktury Stripe można znaleźć w ustawieniach rozliczeń Miro. Dowiedz się [jak znaleźć i pobrać fakturę](01-how-to-find-and-download-an-invoice.md).

## Zrozumienie opłat na fakturze

Twoja następna faktura pokaże wszelkie zmiany, takie jak dodanie lub usunięcie licencji, czy zmiana Twojego abonamentu. Gdy zmienisz abonament, otrzymasz nową fakturę o nazwie **Odnowienie** w swoich ustawieniach rozliczeń.

### Jak prezentują się skorygowane opłaty

Ilekroć wprowadzasz zmiany w swoich licencjach, dodając je lub usuwając, Twoja faktura będzie zawierała dwie dodatkowe linie dla lepszej przejrzystości: **Pozostały czas** i **Niewykorzystany czas**.

- **Pozostały czas** odzwierciedla zaktualizowaną liczbę licencji po recent changes.
- **Niewykorzystany czas** pokazuje liczbę licencji, które miałeś przed wprowadzeniem jakichkolwiek zmian.

Jeśli widzisz opłaty, których nie rozumiesz, sprawdź nasz przewodnik dotyczący [Managing extra licenses](../../administration/user-management/04-manage-extra-licenses.md).

#### Dodawanie licencji

Jeśli dodasz więcej licencji, niż obejmuje Twój bieżący abonament, zostanie naliczona proporcjonalna opłata za każdą dodatkową licencję do końca okresu rozliczeniowego. Na przykład, jeśli dodałeś jedną licencję 23 marca 2021 roku, zobaczysz proporcjonalną opłatę za nią.

![charge_for_an_additional_license.jpg](../../../../../../docs/plans-billing/billing-and-payments/images/21017592958994_charge%20for%20an%20additional%20license.jpg)*Opłata proporcjonalna za dodanie licencji*

#### Usuwanie licencji

Jeśli zaplanowałeś usunięcie licencji, wejdzie ono w życie w dniu odnowienia abonamentu. Aby uzyskać więcej informacji, zobacz [miesięczne i roczne rozliczenia Miro](04-miro-billing.md).

#### Zmiany w Twoim planie

Zmienienie abonamentu Miro lub przejście z miesięcznej na roczną subskrypcję dostosowuje koszt na Twojej następnej fakturze. Każdy niewykorzystany czas z poprzedniego abonamentu zostanie zastosowany do nowej faktury. Na przykład kredyt z niewykorzystanej miesięcznej subskrypcji może być wykorzystany w nowej rocznej subskrypcji.

![amount_for_switch_to_yearly.jpg](../../../../../../docs/plans-billing/billing-and-payments/images/21017605966098_amount%20for%20switch%20to%20yearly.jpg)
*Kredyt za niewykorzystany czas z miesięcznej subskrypcji zastosowany do nowej rocznej subskrypcji*

## Często zadawane pytania

**Jaki jest adres siedziby firmy Miro?**

Nasz adres firmowy znajdziesz na wszystkich fakturach i paragonach Miro:
201 Spear Street Suite 1100 San Francisco, CA, USA 94105

**Czy na moich fakturach wyświetlany jest numer VAT Miro?**

Miro to firma z siedzibą w USA, zarejestrowana do EU VAT w ramach schematu One Stop Shop w Holandii. Miro nie posiada oficjalnego numeru identyfikacyjnego VAT ani specyficznych wymagań dotyczących faktur.
