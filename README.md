#PDFMerger for PHP (PHP 5 Compatible)

Original written by http://pdfmerger.codeplex.com/team/view<br />
Forked from https://github.com/clegginabox/pdf-merger

## Composer Compatible

I've just forked this package to make it compatible with composer

To install add this line to your composer.json

```"choukk/pdf-merger": "dev-master"```

### Example Usage
```php

$pdf = new \Choukk\PDFMerger\PDFMerger;

$pdf->addPDF('samplepdfs/one.pdf', '1, 3, 4');
$pdf->addPDF('samplepdfs/two.pdf', '1-2');
$pdf->addPDF('samplepdfs/three.pdf', 'all');


$pdf->merge('file', 'samplepdfs/TEST2.pdf');

// REPLACE 'file' WITH 'browser', 'download', 'string', or 'file' for output options

// Orientation is no more usefull because it's calculated automatically from PDF width and height (code picked from https://github.com/myokyawhtun/PDFMerger/blob/master/PDFMerger.php)
```
