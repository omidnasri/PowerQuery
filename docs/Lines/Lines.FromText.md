﻿# Lines.FromText
Converts a text value to a list of text values split at lines breaks. If includeLineSeparators is true, then the line break characters are included in the text.
***
function (text as text, optional quoteStyle as nullable any, optional includeLineSeparators as nullable any) as list
***
# Descrition 
Converts a text value to a list of text values split at lines breaks. If includeLineSeparators is true, then the line break characters are included in the text.
        <div>
          <ul>
            <li><code>QuoteStyle.None:</code> (default) No quoting behavior is needed.</li>
            <li><code>QuoteStyle.Csv:</code> Quoting is as per Csv. A double quote character is used to demarcate such regions, and a pair of double quote characters is used to indicate a single double quote character within such a region. </li>
          </ul>
        </div>
    
# Category 
Lines