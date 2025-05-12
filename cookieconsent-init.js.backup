// Cookie Consent Initialisierung
document.addEventListener('DOMContentLoaded', function() {
    // Cookie Consent Einstellungen
    var cc = CookieConsent.run({
        // Locales/Sprache
        language: {
            default: 'de',
            translations: {
                de: {
                    consentModal: {
                        title: 'Wir verwenden Cookies!',
                        description: 'Hallo, diese Website verwendet essenzielle Cookies, um ihren ordnungsgemäßen Betrieb zu gewährleisten, und Tracking-Cookies, um zu verstehen, wie Sie mit ihr interagieren. Letztere werden nur nach Zustimmung gesetzt werden.',
                        acceptAllBtn: 'Alle akzeptieren',
                        acceptNecessaryBtn: 'Alle ablehnen',
                        showPreferencesBtn: 'Einstellungen verwalten',
                        footer: '<a href="/datenschutz">Datenschutzerklärung</a>'
                    },
                    preferencesModal: {
                        title: 'Cookie-Einstellungen',
                        acceptAllBtn: 'Alle akzeptieren',
                        acceptNecessaryBtn: 'Alle ablehnen',
                        savePreferencesBtn: 'Einstellungen speichern',
                        closeIconLabel: 'Schließen',
                        serviceCounterLabel: 'Dienste',
                        sections: [
                            {
                                title: 'Cookie-Verwendung',
                                description: 'Wir verwenden Cookies, um die grundlegenden Funktionen der Website zu gewährleisten und um Ihr Online-Erlebnis zu verbessern. Sie können für jede Kategorie wählen, ob Sie sich an- oder abmelden möchten.'
                            },
                            {
                                title: 'Technisch notwendige Cookies <span class="pm__badge">Immer aktiv</span>',
                                description: 'Diese Cookies sind für das ordnungsgemäße Funktionieren unserer Website unerlässlich. Ohne diese Cookies würde die Website nicht richtig funktionieren.',
                                cookieTable: {
                                    headers: {
                                        name: 'Name',
                                        domain: 'Domain',
                                        description: 'Beschreibung',
                                        expiration: 'Ablauf'
                                    },
                                    body: [
                                        {
                                            name: 'cc_cookie',
                                            domain: 'diese Website',
                                            description: 'Speichert Ihre Cookie-Einstellungen',
                                            expiration: '6 Monate'
                                        }
                                    ]
                                }
                            },
                            {
                                title: 'Analytische Cookies',
                                description: 'Diese Cookies ermöglichen es uns, Besuche und Verkehrsquellen zu zählen, damit wir die Leistung unserer Website messen und verbessern können.',
                                cookieTable: {
                                    headers: {
                                        name: 'Name',
                                        domain: 'Domain',
                                        description: 'Beschreibung',
                                        expiration: 'Ablauf'
                                    },
                                    body: [
                                        {
                                            name: '_ga',
                                            domain: 'diese Website',
                                            description: 'Google Analytics Cookie',
                                            expiration: '2 Jahre'
                                        }
                                    ]
                                },
                                toggle: {
                                    value: 'analytics',
                                    enabled: false,
                                    readonly: false
                                }
                            }
                        ]
                    }
                }
            }
        },
        
        // Kategorien mit entsprechenden Cookies
        categories: {
            necessary: {
                enabled: true,  // Diese Kategorie ist standardmäßig aktiviert und kann nicht deaktiviert werden
                readOnly: true  // Der Benutzer kann diese Kategorie nicht deaktivieren
            },
            analytics: {
                enabled: false, // Diese Kategorie ist standardmäßig deaktiviert
                readOnly: false, // Der Benutzer kann diese Kategorie aktivieren/deaktivieren
                autoClear: {
                    cookies: [
                        {
                            name: '_ga',        // Löscht Cookies, die mit '_ga' beginnen
                            domain: location.hostname,
                            path: '/'
                        }
                    ]
                }
            }
        },
        
        // Layout und GUI
        guiOptions: {
            consentModal: {
                layout: 'box',
                position: 'bottom right',
                equalWeightButtons: true,
                flipButtons: false
            },
            preferencesModal: {
                layout: 'box',
                equalWeightButtons: true,
                flipButtons: false
            }
        }
    });
}); 