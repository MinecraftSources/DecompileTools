# DecompileTools
Tools that help decompile minecraft

Usage

1) Create SRG mappings for obfuscated enum names
enumfixer {jarfile} {output}

2) Create SRG mappings to rename all classes at root level to the following format class_{class}, for inner: class_{class}_in_class_{outer}
mappings {jarfile} {output}

3) Create finder entries for usage with classfinder. Will scan every class ConstantPool, and then will create a mapping that allows to identify this class among the others.
classfindermappings {jarfile} {entrynamestart} {output}

4) Apply finder entries to jar to generate SRG names based on found classes
classfinder {jarfile} {finderentriesfile} {output}
