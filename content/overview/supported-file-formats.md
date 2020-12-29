---
title: Formats de fichier supprotés
id: supported-file-formats
draft: false
weight: 20
author: "people"
---

Darktable supporte un grand nombre de formats de fichiers de divers fabricants de caméras. En outre, darktable peut lire des images spécifiques à faible plage dynamique et à haute plage dynamique – principalement pour l’échange de données entre darktable et d’autres logiciel.

Pour que Darktable puisse considérer un fichier pour l’importation, il doit avoir l’une des extensions suivantes (case independent): `3FR, ARI, ARW, BAY, BMQ, CAP, CINE, CR2, CRW, CS1, DC2, DCR, DNG, GPR, ERF, FFF, EXR, IA, IIQ, JPEG, JPG, K25, KC2, KDC, MDC, MEF, MOS, MRW, NEF, NRW, ORF, PEF, PFM, PNG, PXN, QTK, RAF, RAW, RDC, RW1, RW2, SR2, SRF, SRW, STI, TIF, TIFF, X3F`

Si Darktable a été compilé avec le support JPEG2000, les extensions suivantes sont également reconnues: `J2C, J2K, JP2, JPC`.

Si Darktable a été compilé avec le support GraphicsMagick, les extensions suivantes sont reconnues en plus des extensions standard: `BMP, DCM, GIF, JNG, JPC, JP2, MIFF, MNG, PBM, PGM, PNM, PPM`.

# camera raw files

darktable reads raw files using the open source library [RawSpeed](https://github.com/darktable-org/rawspeed), originally developed by Klaus Post and now maintained as part of the darktable project. The number of supported cameras and file formats is constantly increasing. Most modern camera models are supported, and new ones tend to get added very quickly. It is beyond the scope of this manual to give an exhaustive list.

With the exception of Fujifilm X-Trans cameras, darktable does not decode images from cameras with non-Bayer sensors (e.g. Sigma cameras with the Foveon X3 sensor).

# other image files

darktable natively reads “ordinary” images in JPEG, 8-bit/16-bit PNG and 8-bit/16-bit TIFF format, as well as 16-bit/23-bit floating poing TIFF formats. JPEG2000 is also supported if the required libraries are present at compile time. Similarly, if darktable was compiled with GraphicsMagick support, there are further supported formats, such as GIF, Dicom DCM, additional "exotic" TIFF formats, and some of Sun's “portable xyz-map” family.

darktable also reads high dynamic range images in OpenEXR, RGBE and PFM formats.
