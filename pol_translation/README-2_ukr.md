# Dokumentacja Linea

[Linea](https://linea.build/) to gotowa do użycia sieć warstwy 2, skalująca Ethereum poprzez dostarczanie środowiska równoważnego Ethereum, w którym można wykonywać transakcje, które są następnie przesyłane do Ethereum Mainnet za pomocą rollupu zero-knowledge.

To repozytorium dokumentacji jest zbudowane przy użyciu [Docusaurus](https://docusaurus.io/), a sama strona jest opublikowana pod adresem [`docs.linea.build`](https://docs.linea.build/).

Zobacz [więcej](https://docs-template.consensys.net/) informacji na temat tego, jak Consensys używa Docusaurus.

## Współpraca przy dokumentacji

Zauważyłeś coś brakującego? Błąd w naszej dokumentacji? Utwórz zgłoszenie [tutaj](https://github.com/Consensys/doc.linea/issues).

Alternatywnie, pomóż nam poprawić naszą dokumentację! [Forkuj nasze repo](https://github.com/ConsenSys/doc.linea/fork),
utwórz pull request i oznacz nas do recenzji! (aby uzyskać pomoc w tym zakresie, zobacz  [poniżej](#how-to-submit-a-suggestion-or-change)).

Sprawdź niektóre [dobrze zacząć](https://github.com/ConsenSys/doc.linea/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) problemy, aby zacząć.

### Jak zasugerować zmianę lub dodać coś nowego

Najlepszym sposobem zasugerowania zmiany w tych dokumentach jest proces znany jako **pull request**.
Jeśli nie jesteś zaznajomiony z tym, jak to działa, zapoznaj się z [przewodnikiem GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

Jeśli zamierzasz złożyć pull request, proszę najpierw otworzyć zgłoszenie i [linkować do niego w swoim pull requeście](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue). **est to szczególnie ważne, jeśli jesteś uczestnikiem ekosystemu** —
złożenie szczegółów w zgłoszeniu najpierw ułatwi naszemu zespołowi dokumentacyjnemu przetworzenie Twoich wkładów.

Jeśli ten proces jest zbyt skomplikowany, zawsze możesz otworzyć wątek na [ forum społecznościowym](https://community.linea.build/),
lub zgłosić bilet na [stronie wsparcia](https://support.linea.build/hc/en-us).

Jeśli jesteś zaznajomiony z tworzeniem pull requestów, **zdecydowanie zalecamy uruchomienie wersji tych dokumentów lokalnie i podglądanie swoich zmian lokalnie przed ich przesłaniem**.
W rzeczywistości jest to część procesu PR.

### Współpraca przy poradnikach społecznościowych

eśli stworzyłeś lub zamierzasz stworzyć rozbudowane przewodniki i tutoriale, chętnie przedstawimy Twoje treści
w naszej [sekcji poradników społecznościowych](developers/guides/community).

Najpierw stwórz zgłoszenie opisujące treści, które chciałbyś zobaczyć dodane lub które zamierzasz dodać. Jeśli reprezentujesz organizację (taką jak dapp), proszę skorzystać z formularza zgłoszeniowego dla wkładów ekosystemowych.

Kiedy będziesz gotowy do rozpoczęcia pracy, [forkuj nasze repo](https://github.com/Consensys/doc.linea/fork),
stwórz pull request i oznacz nas do recenzji!

### Współpraca przy słowniczku zero-knowledge

Zanurzasz się w rollupy zero-knowledge i utknąłeś na technicznej terminologii? Rozpoczęliśmy
open source słowniczek Zero-Knowledge, aby zdefiniować niektóre powszechne terminy, które możesz napotkać, zanurkując
w krajobraz L2.

[Forkuj nasze repo](https://github.com/Consensys/doc.linea/fork), i dodaj termin w porządku alfabetycznym
do `docs/reference/glossary.md`. Następnie zrób pull request i oznacz nas do recenzji!

### Dodatkowe zasoby

Zapoznaj się z [wytycznymi dotyczącymi wkładów w dokumentację Consensys](https://docs-template.consensys.net/) aby uzyskać informacje na temat:

- [Składania wkładu](https://docs-template.consensys.net/contribute/submit-a-contribution) za pomocą forków i pull requestów.
- Konsultacji [przewodnika stylu dokumentacji.](https://docs-template.consensys.net/contribute/style-guide).
- [Poprawnego formatowania Markdown](https://docs-template.consensys.net/contribute/format-markdown).
- [Podglądania dokumentacji](https://docs-template.consensys.net/contribute/preview) lokalnie.

## Uruchamianie lokalnie

Będziesz potrzebować **Node.js** do uruchomienia podglądów na żywo dokumentacji lokalnie.



Zdecydowanie zaleca się użycie narzędzia takiego jak  [`nvm`](https://github.com/nvm-sh/nvm#installing-and-updating)
do zarządzania wersjami Node.js na swoim komputerze.

### Instalowanie zalecanej wersji Node.js za pomocą `nvm`

1. Postępuj zgodnie z powyższymi instrukcjami, aby zainstalować  `nvm` na swoim komputerze, lub przejdź [ tutaj](https://github.com/nvm-sh/nvm#installing-and-updating).
2. Przejdź do folderu głównego projektu w terminalu.
3. Uruchom `nvm install` a następnie `nvm use`. To zainstaluje wersję określoną przez ten projekt w pliku `.nvmrc`.

### Uruchamianie projektu

1. Przejdź do folderu głównego projektu po zainstalowaniu Node.js.
2. Uruchom poniższe polecenia w kolejności, co jest wymagane tylko raz:

   ```bash
   npm install
   npm run prepare
   ```

3. Aby uzyskać podgląd i za każdym razem później:

   ```bash
   npm run start
   ```

### Budowanie

    $ npm run build

To polecenie generuje statyczne treści w katalogu `build`  które można udostępniać za pomocą dowolnej usługi hostingu treści statycznych.

### Dodawanie nowych słów do słownika

To repozytorium zawiera _linter_, który możesz traktować jako sprawdzanie pisowni, które również sprawdza formatowanie kodu i standardy, i wiele więcej. Możliwe jest, że użyjesz słowa w swojej treści, które nie jest znane linterowi, a twoje budowanie lub commit zakończy się niepowodzeniem.

Możesz uruchomić linter w każdej chwili za pomocą polecenia `npm run lint`.

Jeśli linter znajdzie słowo, którego nie rozpoznaje, sprawdź `project-words.txt` iw katalogu głównym; jeśli słowo, które linter wychwycił, jest poprawnie napisane i chcesz, aby przeszło test lintera, dodaj je do `project-words.txt`,  zapisz, dodaj i commituj te zmiany, a następnie sprawdź, czy przechodzi.

Dla porządku upewnij się, że przestrzegasz alfabetycznego porządku ustanowionego w `project-words.txt`.
