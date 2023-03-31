function Get-Cases ($string, $prefix=@())
{
  if ($string -eq '') {
     return -join $prefix
  }
  Get-Cases $string.Substring(1) ($prefix + $string.Substring(0, 1).ToLower())
  Get-Cases $string.Substring(1) ($prefix + $string.Substring(0, 1).ToUpper())
}

Get-Cases 'caseblaster'
