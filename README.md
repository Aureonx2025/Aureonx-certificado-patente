# Certificado Técnico de Invención - AUREONX

📄 Documento: [Descargar PDF](# Reintentar guardado quitando caracteres no compatibles con latin-1 (como el punto medio "•")

class CertPDFFixed(FPDF):
    def header(self):
        pass
    def footer(self):
        self.set_y(-15)
        self.set_font("Arial", "I", 8)
        self.set_text_color(150, 150, 150)
        self.cell(0, 10, "AUREONX - Protección técnica temporal con DID descentralizado", 0, 0, 'C')

# Nuevo PDF con texto corregido
pdf = CertPDFFixed()
pdf.add_page()
pdf.image(imagen_path, x=10, y=10, w=190)
pdf.add_page()

pdf.set_font("Arial", "B", 14)
pdf.set_text_color(0, 51, 102)
pdf.cell(0, 10, "Registro Técnico Vinculado a DID Descentralizado", ln=True)

pdf.set_font("Arial", "", 12)
pdf.set_text_color(0)
pdf.ln(5)
pdf.cell(0, 10, f"Número de patente visible: {numero_patente}", ln=True)
pdf.cell(0, 10, f"Fecha de emisión: 21 de mayo de 2025", ln=True)
pdf.cell(0, 10, f"DID asociado: {did}", ln=True)

pdf.ln(10)
pdf.multi_cell(0, 10,
    "Este documento vincula de forma pública y permanente la patente presentada anteriormente con una identidad digital "
    "descentralizada (DID) bajo el estándar W3C. Esta firma permite a cualquier auditor verificar la autoría, fecha y asociación "
    "con AUREONX sin depender de terceros, manteniendo trazabilidad en redes públicas como IPFS o blockchains.")

pdf.ln(10)
pdf.set_font("Arial", "I", 11)
pdf.cell(0, 10, "Este documento puede ahora ser publicado en plataformas públicas como Arweave, IPFS, GitHub o redes sociales como prueba técnica de autoría.", ln=True)

# Guardar el nuevo PDF
final_pdf_path_fixed = "/mnt/data/AUREONX_certificado_DID_con_imagen_final.pdf"
pdf.output(final_pdf_path_fixed)

final_pdf_path_fixed)

**Número de patente referencial**: 208131  
**Fecha de emisión**: 21 de mayo de 2025  
**Inventores**:  
- Luis Fernando Alexander Palomo Maurera  
- Andrés Felipe Sánchez Sánchez

---

## DID (Decentralized Identifier)

Este documento está firmado y vinculado con la siguiente identidad descentralizada (DID)
:
