ExtraAssignment-Sequence-Aligner
================================
chimp = 'gagcagctgaacaagctgatgaccaccctccatagcaccgcaccccattttgtccgctgtattatccccaatgagtttaagcaatcgg'
human = 'gagcagctgaacaagctgatgaccaccctccatagccgcaccccattttgtccgctgtattatccccaatgagtttaagcaatcgg'
print len(chimp)
print len(human)
#index == length of the smaller sequence
def comparison(list1, list2, index):
    while True:
        if index == 0:
            break
            
        elif list1[index] == list2[index]:
            comparison(list1, list2, index - 1)
        elif list1[index] != list2[index]:
            print str(index) + list1[index] + list2[index]
            comparison(list1, list2, index-1)
        break

