---
external help file: Microsoft.Exchange.TransportMailflow-Help.xml
online version: https://docs.microsoft.com/powershell/module/exchange/set-recordreviewnotificationtemplateconfig
applicable: Security & Compliance Center
title: Set-RecordReviewNotificationTemplateConfig
schema: 2.0.0
author: chrisda
ms.author: chrisda
ms.reviewer:
---

# Set-RecordReviewNotificationTemplateConfig

## SYNOPSIS
This cmdlet is available only in the cloud-based service.

Use the Set-RecordReviewNotificationTemplateConfig cmdlet to set up the customized record review notification and reminder that's sent when an item requires review.

For information about the parameter sets in the Syntax section below, see [Exchange cmdlet syntax](https://docs.microsoft.com/powershell/exchange/exchange-cmdlet-syntax).

## SYNTAX

```
Set-RecordReviewNotificationTemplateConfig -IsCustomizedNotificationTemplate <Boolean> -IsCustomizedReminderTemplate <Boolean>
 [-CustomizedNotificationDataString <String>]
 [-CustomizedReminderDataString <String>]
 [<CommonParameters>]
```

## DESCRIPTION
To use this cmdlet in Security & Compliance Center PowerShell, you need to be assigned permissions. For more information, see [Permissions in the Microsoft 365 compliance center](https://docs.microsoft.com/microsoft-365/compliance/microsoft-365-compliance-center-permissions).

## EXAMPLES

### Example 1
```powershell
Set-RecordReviewNotificationTemplateConfig -IsCustomizedNotificationTemplate $true -CustomizedNotificationDataString "This is the Contoso notification" -IsCustomizedReminderTemplate $true -CustomizedReminderDataString "This is the Contoso reminder"
```

This example configures customized review notification text and review reminder text.

## PARAMETERS

### -IsCustomizedNotificationTemplate
The IsCustomizedNotificationTemplate switch specifies whether to use a customized review notification instead of the system default notification. Valid values are:

- $true: Use a customized review notification. You specify the notification text using the CustomizedNotificationDataString parameter.
- $false: Use the default system notification. This is the default value.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:
Applicable: Security & Compliance Center

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsCustomizedReminderTemplate
The IsCustomizedReminderTemplate switch specifies whether to use a customized review reminder instead of the system default reminder:

- $true: Use a customized review reminder. You specify the reminder text using the CustomizedReminderDataString parameter.
- $false: Use the default system reminder. This is the default value.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:
Applicable: Security & Compliance Center

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomizedNotificationDataString
The CustomizedNotificationDataString parameter specifies the customized review notification text to use. If the value contains spaces, enclose the value in quotation marks (").

The value of this parameter is meaningful only when the value of the IsCustomizedNotificationTemplate parameter is $true.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Security & Compliance Center

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CustomizedReminderDataString
The CustomizedReminderDataString parameter specifies the customized review reminder text to use. If the value contains spaces, enclose the value in quotation marks (").

The value of this parameter is meaningful only when the value of the IsCustomizedReminderTemplate parameter is $true.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Security & Compliance Center

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

###  

## OUTPUTS

###  

## NOTES

## RELATED LINKS
